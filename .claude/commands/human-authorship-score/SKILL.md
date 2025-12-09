---
name: human-authorship-score
description: Review articles and score their "human authorship" on a 0-100 scale. Use when asked to evaluate writing for AI patterns, score human voice, detect AI-generated content, check if writing sounds human, or review articles for authenticity. Identifies AI writing patterns, flags specific passages, and provides rewrite guidance.
---

# Human Authorship Score

Evaluate writing to determine how "human" it reads. Score from 0 (AI slop) to 100 (distinctly human).

## Workflow

### Step 1: Determine Genre

Before scoring, classify the content:

| Genre | Description | Scoring Adjustments |
|-------|-------------|---------------------|
| **Essay/Opinion** | Personal perspective, argument | Full scoring, all components weighted normally |
| **Tutorial** | How-to, instructional | Lower Voice weight (15%), higher Specificity (30%) |
| **Reference** | Documentation, specs | Lower Stance (15%), Voice (10%); higher Specificity (35%) |
| **Narrative** | Story-driven, case study | Higher Voice (25%), Opening (20%) |
| **News/Report** | Factual reporting | Lower Voice (10%), higher Specificity (35%) |

State the detected genre before scoring.

### Step 2: Score Components

See `references/scoring-rubric.md` for detailed criteria.

| Component | Default Weight | Measures |
|-----------|----------------|----------|
| **Stance** | 20% | Position-taking, recommendations, claims |
| **Specificity** | 20% | Personal experience, real numbers, named failures |
| **Voice** | 20% | Contractions, asides, personality, tonal consistency |
| **Formatting** | 15% | Absence of AI formatting tells (emojis, excessive structure) |
| **Opening** | 12.5% | Story/problem/opinion vs. throat-clearing |
| **Closing** | 12.5% | Opinion/next step/question vs. "In conclusion" |

Each component: 0-100 score.

### Step 3: Calculate Overall Score

```
Overall = (Stance × weight) + (Specificity × weight) + (Voice × weight) + (Formatting × weight) + (Opening × weight) + (Closing × weight)
```

### Step 4: Assign Confidence

| Confidence | Criteria |
|------------|----------|
| 85-100% | Clear signals (obvious AI patterns OR strong human voice) |
| 70-84% | Moderate signals, some ambiguity |
| 50-69% | Mixed signals, possibly edited AI or bland human |
| <50% | Insufficient signals to judge reliably |

### Step 5: Generate Output

Use this exact format:

```
HUMAN AUTHORSHIP SCORE: [score]/100
Confidence: [confidence]%
Genre: [detected genre]

COMPONENT BREAKDOWN:
├── Stance:      [score]/100  — [one-line rationale]
├── Specificity: [score]/100  — [one-line rationale]
├── Voice:       [score]/100  — [one-line rationale]
├── Formatting:  [score]/100  — [one-line rationale]
├── Opening:     [score]/100  — [one-line rationale]
└── Closing:     [score]/100  — [one-line rationale]

FLAGGED PASSAGES:
[Number each. Quote the passage, then explain the problem and suggest fix.]

1. "[exact quote]"
   → [Pattern name]. [Why it fails]. [Specific fix].

2. "[exact quote]"
   → [Pattern name]. [Why it fails]. [Specific fix].

[Continue for all flagged passages, typically 3-6]

MISSING HUMAN SIGNALS:
- [What's absent that a human would include]
- [Be specific: numbers, failures, opinions, stories]

REWRITE PRIORITIES:
1. [Most important fix with specific suggestion]
2. [Second priority with example]
3. [Third priority with example]

VERDICT: [Based on score threshold]
```

### Verdict Thresholds

Be brutal. No softening. The writer needs to hear it.

| Score | Verdict |
|-------|---------|
| 80-100 | "Ship it." |
| 60-79 | "You wrote it, but you let the robot polish away your personality. Put yourself back in." |
| 40-59 | "This is a human holding a robot's hand. Decide who's writing this and commit." |
| 20-39 | "AI slop with a human byline. You're laundering robot words. Write it yourself or don't publish." |
| 0-19 | "This is ChatGPT output. You didn't write this. Don't pretend you did." |

## Pattern Detection

### AI Patterns (Lower Scores)

**Voice patterns:**
- Sycophantic openers: "That's a great question!"
- Hedge stacking: "It's important to note that it may be worth considering..."
- Neurotically positive: everything is "exciting," "powerful," "game-changing"
- False enthusiasm: "Let's dive in!" / "Let's explore!"

**Structure patterns:**
- Throat-clearing: "In today's fast-paced world..."
- Everything for beginners: explaining basics to advanced audience
- Compulsive completeness: every edge case, every caveat
- Symmetric false balance: "On one hand... on the other hand... it depends"

**Detail patterns:**
- Redundant pairs: "each and every," "first and foremost"
- Explaining the obvious: "This is important because it matters"
- Defensive citations: supporting claims no one disputes
- List bloat: 10 items when 3 make the point

**Opening patterns (AI):**
- Definition lead: "X is defined as..."
- "In today's world/landscape/era..."
- "This article will explore..."
- Preview without payoff

**Closing patterns (AI):**
- "In conclusion..."
- Summary of what was just said
- "By implementing these best practices..."
- Generic call to action

**Formatting patterns (AI):**

*Emoji abuse:*
- Excessive emojis: 🚀📊💡🔥 scattered throughout
- Emoji bullet points: ✅ or ➡️ instead of regular bullets
- Formulaic emoji placement: emoji at start of every header or list item
- "# ✅ Section Title" pattern — dead giveaway

*Punctuation tells:*
- Em dash overuse: one is fine, but "word — and another — thing" triple-dashing is AI
- Note: en dash (–) is normal; em dash (—) abuse is the tell
- Semicolon overuse in casual writing

*Copy-paste laziness:*
- Raw markdown visible: ``` or # or ** in published content
- Unicode bold characters (𝗯𝗼𝗹𝗱) instead of actual formatting
- Non-standard fonts or symbols that don't render properly
- Obvious ChatGPT artifacts: "As an AI language model..." or "I'd be happy to help!"

*Structure tells:*
- Over-structured: every paragraph has a heading
- Numbered lists for everything (even non-sequential content)
- Bold/italic overuse: **every** *other* **word** emphasized
- "Key takeaways" boxes that repeat the content
- Section headers that are questions ("What is X?")
- Excessive whitespace between every element
- Tables where prose would suffice

*The "helpful AI" signature:*
```
# ✅ Next Step For Readers:
You don't need to learn all 10 deeply right now.
Start small — pick 2 or 3 that match your goals:
```
This pattern (emoji header + reassurance + em dash + colon-terminated suggestion) is a dead giveaway. Humans don't write like this.

### Human Patterns (Higher Scores)

**Voice patterns:**
- Contractions used naturally
- Asides and personality
- Specific phrasing choices
- Tonal consistency throughout

**Stance patterns:**
- Clear thesis stated
- Recommendations made
- Positions defended
- Willing to be wrong

**Specificity patterns:**
- Personal experience referenced
- Specific numbers from real situations
- Named failures ("We tried X, it broke because...")
- Concrete examples from actual work

**Opening patterns (Human):**
- Story or specific problem
- Opinion stated upfront
- Surprising fact or claim

**Closing patterns (Human):**
- Opinion or recommendation
- Specific next step
- Open question for reader
- "If I were starting over, I'd..."

**Formatting patterns (Human):**
- Minimal emoji use (or none)
- Structure serves content (not vice versa)
- Lists only when content is actually a list
- Emphasis used sparingly for genuine importance
- Prose paragraphs that flow naturally
- Headers that organize (not fragment) the narrative
- Code blocks only for actual code
- Whitespace that aids reading (not padding)
