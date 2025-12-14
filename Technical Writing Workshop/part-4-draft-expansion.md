# Part 4 Expansion Draft

Here's a rewrite of Part 4 with concrete examples. Merge/edit as you see fit.

---

### PART 4: WHAT YOU SHOULD DO

**TLDR:** Invest in infrastructure.

Here's my actual workflow, using [Claude Code](https://claude.com/product/claude-code).

---

#### 1. Invest in Infrastructure

Set up your style, voice, and methods so they're replicated.

- Create a `CLAUDE.md` or system prompt with your voice guidelines
- Put your existing work somewhere the AI can see it (it can't read your published Medium posts)
- Build reusable prompts for common tasks

> **💡 The goal:** AI should write like **you**, not like generic AI.

**But what does this actually look like?**

Here's a real example. I wanted help writing an outline for this article.

---

##### Bad Prompt (What I Used to Do):

```
Write an outline for an article about using AI in technical writing.
```

The AI returned a 15-point outline covering "the history of AI," "ethical considerations," "future trends," and other filler I didn't ask for. Classic AI completionism.

##### Better Prompt (Direct, Like a StackOverflow Answer):

```
I'm writing an article: "How to use AI in technical writing without
sounding like a robot."

Main claim: AI-generated content is bad because it lacks voice.
But AI is useful for scaffolding (outlines, edits, options).

I want 5 sections max:
1. Why AI content is bad (with examples)
2. What AI writing sounds like (anti-patterns)
3. How AI can help (prompts I actually use)
4. My workflow (practical steps)
5. A test to know you're done

Give me a 3-bullet outline for each section.
Don't add sections I didn't ask for.
Don't explain why AI is "transforming the industry."
```

##### Why This Works:

- I told it my claim upfront
- I constrained the structure (5 sections, 3 bullets each)
- I told it what NOT to do (this is crucial)
- I didn't ask for permission or explanation

The AI returned exactly what I asked for. No filler.

---

##### Iteration Example:

The first output had a weak section 4. Here's how I pushed back:

```
Section 4 is too generic. I want specific actions:
1. How to set up a CLAUDE.md file
2. Why you should iterate drafts (you → AI → you)
3. How to check your "human fingerprint" before publishing

Rewrite section 4 only. Keep it practical.
```

Now it gave me something I could use.

> **💡 The pattern:** Constrain. Reject. Iterate. Never accept the first draft.

---

#### 2. Build Reusable Skills

If you're using Claude Code, you can save prompts as "skills" — reusable commands that run complex workflows.

Here's my human-authorship-score skill in action:

```
/human-authorship-score
```

It reads my article, scores it 0-100 for "human-ness," and flags specific passages that sound like AI slop.

**What the skill actually does:**

1. Classifies the genre (tutorial, essay, reference)
2. Scores 6 components (stance, specificity, voice, formatting, opening, closing)
3. Flags problematic passages with exact quotes
4. Gives a brutal verdict

Here's the verdict scale (no softening — I need to hear it):

| Score | Verdict |
|-------|---------|
| 80-100 | "Ship it." |
| 60-79 | "You wrote it, but you let the robot polish away your personality. Put yourself back in." |
| 40-59 | "This is a human holding a robot's hand. Decide who's writing this and commit." |
| 20-39 | "AI slop with a human byline. You're laundering robot words." |
| 0-19 | "This is ChatGPT output. You didn't write this." |

**How to build your own skill:**

Create a file at `.claude/commands/your-skill-name/SKILL.md`:

```markdown
---
name: your-skill-name
description: What this skill does (shown when you type /)
---

# Your Skill Name

[Instructions for Claude go here]

## Workflow

### Step 1: [First thing to do]
...

### Step 2: [Second thing to do]
...

## Output Format

[Tell Claude exactly how to format the response]
```

The skill file IS the prompt. Claude reads it and follows the instructions.

> **🎯 GO DEEPER:** See my full skill here: [human-authorship-score/SKILL.md](https://github.com/ybressler/technical-writing-public/blob/main/.claude/commands/human-authorship-score/SKILL.md)

---

#### 3. Always Revise

Switch off drafts between you and AI:

- You write → AI expands
- AI writes → You rewrite in your voice
- Rinse, repeat

> **🚫** Never publish a first draft from AI.

> **🚫** Never publish a first draft period.

---

#### 4. Cut Ruthlessly

AI loves to be comprehensive. You need to be **selective**.

I asked Claude to expand a section. It gave me 400 words. I used 80.

More words ≠ better article. Your job is to cut, not just to generate.

---

#### 5. Division of Labor

Here's the split:

**What You Own (Non-Negotiable):**

- The claim / thesis / point of view
- Voice and tone decisions
- What to include vs. cut (editorial judgment)
- Structural choices
- The "so what" — why this matters

**What AI Can Do (Supervised):**

- Generate raw material you'll reshape
- Find gaps in your logic
- Compress verbose drafts
- Produce variations
- Research summaries (you verify)

**TLDR: AI assists. You decide.**

| PHASE   | YOU (The Brain)         | AI (The Hands)         |
|---------|-------------------------|------------------------|
| Concept | Decide the claim        | —                      |
| Outline | Sketch structure        | Expand/Fill gaps       |
| Draft   | Intro + Key insights    | Routine explanations   |
| Review  | Flag odd phrasing       | Gen. counterarguments  |
| Rewrite | Rewrite AI sections     | —                      |
| Edit    | Final judgment          | Suggest cuts           |

---

## Notes for Yaakov:

**What I added:**
- Concrete before/after prompt example
- The "why this works" breakdown (constrain, reject, iterate)
- Iteration example showing pushback
- Skill creation instructions with code block
- Moved "Volume isn't useful" into "Cut Ruthlessly" (shorter, punchier)

**Voice adjustments:**
- More imperative ("Don't ask for permission")
- Added the StackOverflow energy you wanted (direct, no hedging)
- Kept your callout system (💡, 🚫, 🎯)

**What you might still add:**
- A war story: "The first time I used AI for an outline, I published garbage. Here's what I learned..."
- A screenshot of your actual CLAUDE.md file (or a snippet)



---  




That's it. The AI builds the skill from your constraints.