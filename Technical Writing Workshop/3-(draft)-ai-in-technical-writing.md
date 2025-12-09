# AI in Technical Writing
## Good ways to use AI and bad ways to use AI.

---

# I. THE BAD

*Things to avoid when using AI for writing.*

<p align="center">
<img src="../Images/michael-scott-junior.jpeg" alt="Michael Scott presenting" width="400"><br>
<em>"I'm not superstitious, but I am a little stitious." — The energy we're avoiding.</em>
</p>

---

## The "Whitewashed Voice"

AI writing sounds like... AI writing.

Let me show you what I mean.

---

### Example: Formulaic and Robotic

```text
Memory management is vital in any data processing system, and its importance escalates when dealing with big data. In Apache Spark, grasping the fundamentals of in-memory processing is key to optimizing performance. Here's my consolidated understanding:

There are different level of memory management in Spark
	1. On-Heap Memory
	2. Overhead memory
	3. Off -Heap Memory
```

**What's wrong:** This is a Wikipedia stub pretending to be an article.

placeholder phrases that say nothing:
*` "Vital"`
* `"importance escalates,"`
* `"grasping the fundamentals"`

`"Here's my consolidated understanding"` promises personal insight, then delivers a bullet list. ***The author has no point of view*. They're just... listing things.**



---

### Example: Neurotically Positive

> In today's ==rapidly evolving== landscape of data engineering, it's ==incredibly exciting== to explore the ==powerful possibilities== that ==modern tools== bring to your workflow. These ==game-changing technologies== offer ==transformative potential== for teams looking to enhance their productivity.

**What's wrong:** Count the empty superlatives: `["exciting", "powerful", "game-changing", "transformative"]`

<u>None of these words communicate anything specific.</u> This is hype without substance. A reader learns nothing except that the author is enthusiastic (or pretending to be).

---

### Example: Hedge Stacking

> ==It's important to note== that while there ==may be== some ==potential benefits== to this approach, ==it's worth considering== that results ==can vary== depending on your specific use case. That said, it ==might be helpful== to explore these options further.

**What's wrong:** This sentence commits to nothing. `["Important to note," "may be," "potential," "worth considering," "can vary," "might be helpful"]` — the author is backing away from every claim before making it. <u>If you're not willing to say something definite, why are you writing?</u>

---

### Example: Throat-Clearing Introduction

> In today's fast-paced world of software development, efficient data processing has become more critical than ever. As organizations increasingly rely on data-driven decision making, understanding the tools and techniques available has never been more important.

**What's wrong:** This is the written equivalent of someone saying "um" for 30 seconds before getting to their point. The reader already knows data is important — that's why they clicked on your article. Skip the preamble. Start with your actual point.

---

## Voice Problems

| Pattern | Example | Why it fails |
|---------|---------|--------------|
| **Sycophantic openers** | "That's a great question!" | Reader isn't asking you to validate them |
| **Hedge stacking** | "It may be worth considering..." | Says nothing, burns trust |
| **Neurotically positive** | Everything is "exciting," "powerful" | No credibility, no contrast |
| **False enthusiasm** | "Let's dive in!" | Filler energy, no substance |

---

## Voice Problems: An Analogy

Imagine hiring a tour guide.

**Bad tour guide (AI voice):**
> "Welcome! This is going to be an exciting journey! The museum is a truly remarkable institution with many important exhibits. Let's explore the fascinating world of art together!"

**Good tour guide (human voice):**
> "Skip the first three rooms — they're renovation leftovers. But room 4 has a Vermeer they acquired last year that nobody knows about. I'll show you the angle where you can see his signature hidden in the tablecloth."

The bad guide tells you everything is important.
The good guide tells you what *actually* matters.

---

More examples:

| Bad Tour Guide (AI) | Good Tour Guide (Human) |
|---------------------|-------------------------|
| "The café offers a variety of dining options to suit every taste!" | "The café is overpriced. There's a sandwich cart outside Gate B — half the price, twice as good." |
| "This painting is considered by many to be an important work." | "This painting is mid. But the one behind you? The artist painted it while dying of tuberculosis. Look at the brushwork — you can see his hand shaking." |
| "Be sure to check out all the gift shops for unique souvenirs!" | "The gift shop on floor 2 has the same postcards for $2 less." |
| "There are restrooms conveniently located throughout the museum." | "Use the bathroom on floor 3. The ones by the entrance always have a line." |
| "The collection spans many centuries of artistic achievement." | "Ignore the Renaissance wing unless you like crowds. Back stairwell — unmarked room with medieval manuscripts, zero tourists." |

The pattern: **Bad guides describe. Good guides recommend.**

AI describes because it has no idea what matters. You do.

---

### "But I Have to Cover the Required Material"

Fair. Sometimes tour guides *must* read from a script. The museum requires them to mention the founding date, the donor names, the fire safety exits.

Good guides still find ways to add value:

| Required Script | How a Good Guide Augments It |
|-----------------|------------------------------|
| "The museum was founded in 1923 by Margaret Whitfield." | "Founded in 1923 — but here's the thing: Margaret Whitfield hated most of the art she donated. She bought it to spite her ex-husband's taste. That's why the collection is so eclectic." |
| "Please note the emergency exits located on your left and right." | "Exits are there and there. Also, if the fire alarm goes off, don't panic — it's usually the café burning toast. Happened twice last month." |
| "This gallery features works from the Impressionist period." | "Impressionist gallery. If you only have 10 minutes, skip to the back wall. The three Monets in front are fine, but everyone crowds them. The Caillebotte in the corner is better and you'll actually be able to see it." |

The script is the *floor*, not the ceiling.

---

### Tour Guides vs. HR Training

Both have required content. The difference is *why they exist*.

<table>
<tr>
<td width="50%" align="center">
<img src="../Images/abdul-basit-melik-boring-meeting.jpg" alt="Boring corporate meeting" width="100%"><br>
<em>HR Training Energy</em>
</td>
<td width="50%" align="center">
<img src="../Images/bernie-almanzar-tour-guide.jpg" alt="Enthusiastic tour guide" width="100%"><br>
<em>Tour Guide Energy</em>
</td>
</tr>
</table>

**HR training (dress code section):**
> "Employees are expected to maintain professional attire in accordance with company policy guidelines. Clothing should be appropriate for a business environment and consistent with the standards outlined in Section 3.4 of the Employee Handbook. Management reserves the right to determine appropriateness on a case-by-case basis."

**Tour guide (same information):**
> "Wear normal clothes. No bikinis — this is an office, not Miami. If you're unsure, jeans and a polo are fine. Nobody actually cares unless a client is visiting, then throw on something with a collar."

Same topic. Completely different purpose.

**HR training exists to protect the company.**:
* They don't care if you learn.
* They don't care if you enjoy it.
* They need documentation that you were informed, so when something goes wrong, legal can say "the policy was communicated."
* <u>The legalese isn't an accident — it's the point.</u>

**Tour guides exist to serve the audience.**
* They want you to have a good time.
* They want you to learn something.
* They put soul into it because *they actually care whether you get value*.

AI writes like HR training. It covers everything, commits to nothing, and exists to complete the task — not to help you.

**Your job is to be the tour guide.** Write like you give a damn whether the reader learns something.

---

### Reading the Room

Good guides also adjust based on who's in front of them:

| Audience | What a Good Guide Does |
|----------|------------------------|
| **School group (8-year-olds)** | "See this painting? The guy in it farted at a king and got exiled. True story." (Skip the art theory.) |
| **Art history PhD students** | "You'll notice the sfumato technique here differs from his Milan period — happy to go deeper if you want." (Don't explain what sfumato means.) |
| **Tourists with 30 minutes** | "You have half an hour? Here's the only route that matters: Room 4, Room 11, skip the rest. Trust me." |
| **Repeat visitors** | "You've seen the main collection. Want to see the restoration lab? It's not on the public tour but I can get us in." |

AI can't read the room. It doesn't know if the reader is a beginner or an expert, in a hurry or doing deep research, skeptical or already convinced.

**You do.** That's what makes your judgment irreplaceable.

**AI writes like a bad tour guide.** Your job is to be the good one.

---

## Structure Problems

Voice isn't the only issue. AI also structures content poorly.

| Pattern | Example | Why it fails |
|---------|---------|--------------|
| **Throat-clearing intros** | "In today's fast-paced world of data engineering..." | Delays the point, reader skips anyway |
| **Everything for beginners** | Explaining what an API is in an advanced post | Wrong audience, bloat |
| **Compulsive completeness** | Listing every edge case | Buries signal in noise |
| **Symmetric false balance** | "On one hand... on the other... it depends" | Avoids taking a position |

---

## Structure Problems: A Real Example

Let's look at an actual article: [Spark Memory Management and its types](https://medium.com/@vtrkayalrajan/spark-memory-management-and-its-types-425af52d7c15)

**The opening:**
> Memory management is vital in any data processing system, and its importance escalates when dealing with big data. In Apache Spark, grasping the fundamentals of in-memory processing is key to optimizing performance. Here's my consolidated understanding...

**The ending:**
> Hope this story provide basic understanding of the Spark Memory management.

**What's structurally wrong:**

1. **No thesis.** What is this article *arguing*? Nothing. It's just a list of facts with no point of view.

2. **No audience clarity.** It explains what RDDs are (beginner) but then dives into memory fractions and formulas (advanced). Who is this for?

3. **No prioritization.** Three types of memory are listed equally. Which one should I care about? When does each matter? The author won't say.

4. <b>No <u>"so what."</u></b> After 1,000 words of technical detail, the conclusion is "hope this provides basic understanding." What should I *do* with this information? No guidance.

5. **No opinion.** Should I use off-heap memory? When? The article won't commit: "Even though the best performance is obtained when operating solely in on-heap memory, Spark also makes it possible to use off-heap storage for certain operations." That's not advice. That's a shrug.

**The structure problem:** This isn't an article. It's documentation that wandered onto Medium and put on a blog post costume.

---

## Detail Problems

| Pattern | Example | Why it fails |
|---------|---------|--------------|
| **Redundant pairs** | "each and every," "first and foremost" | Empty calories |
| **Explaining the obvious** | "This is important because it matters" | Circular, adds nothing |
| **Defensive citations** | Supporting claims no one disputes | Wastes reader attention |
| **List bloat** | 10 items when 3 make the point | Dilutes impact |

---

## The Real Problem with AI Writing

AI doesn't write to communicate. It writes to *complete the task.*

Ask AI to write about Spark memory management, and it will produce comprehensive coverage of every subtopic. But it won't tell you:
- Which parts actually matter for your use case
- What the author learned the hard way
- Where the documentation is wrong or misleading
- What to do first vs. what to ignore

==**Comprehensiveness is not the same as usefulness.**==

Your readers don't need everything. They need the right things, in the right order, with your judgment about what matters.

---

## Why Does This Matter?

**The real question:**

> People can talk to AI themselves. Why should they read *your* conversation with it?

---

## The Data Says Readers Can Tell

In October 2025, researchers from the University of Maryland and Pangram Labs published ["AI use in American newspapers is widespread, uneven, and rarely disclosed"](https://arxiv.org/abs/2510.18774) — a study of **186,000 articles from 1,500 newspapers**.

**The headline finding:** 9.1% of articles contained AI-generated or mixed content.

But here's what matters for *you*:

| Where | AI Content Rate |
|-------|-----------------|
| News pages (major papers) | 0.7% |
| **Opinion pages (NYT, WSJ, WaPo)** | **4.5%** |

Opinion articles were **6.4x more likely** to contain AI than news articles at the same publications.

**Who's using it?** Mostly guest contributors, not staff writers.

**Who's disclosing it?** Almost nobody.
- Only **5 of 100** manually reviewed articles disclosed AI use
- Only **7 of 1,500** newspapers had public AI policies

> "As a reader, you generally don't have a way to know if the news or opinions come from AI... It makes it hard to trust the factuality of the content."
> — **Mohit Iyyer**, Associate Professor of Computer Science, UMD (senior author)

The detection tools are getting better. Readers are getting skeptical. And when they spot AI slop? They leave.

**Your voice is your value.** If readers wanted generic AI output, they'd generate it themselves.

---

**Sources:**
- [Full paper (arXiv)](https://arxiv.org/abs/2510.18774)
- [UMD press release](https://today.umd.edu/report-ai-use-in-newspapers-is-widespread-uneven-and-rarely-disclosed)
- [TechXplore coverage](https://techxplore.com/news/2025-10-extent-ai-content-american-news.html)

---

## 🔴 Exercise: Spot the Slop

*Let's practice identifying AI patterns.*

---

### Example 1: The Classic Throat-Clear

```
In today's rapidly evolving landscape of data engineering, it's important
to note that leveraging AI tools can be a powerful way to enhance your
workflow. Let's dive in and explore how you can use these exciting
technologies to boost your productivity. First and foremost, it's worth
considering that each and every data engineer should...
```

> [!PROBLEMS]-
 > **Problems:**
 >* Throat-clearing intro
 >* false enthusiasm `("Let's dive in!")`
 >* hedge stacking ("it's important to note," "it's worth considering")
 >* redundant pairs ("each and every," "first and foremost")
 >* neurotically positive ("exciting," "powerful").

---

### Example 2: The False Balance

```
There are several approaches to handling this problem. On one hand, you
could use Option A, which has certain advantages. On the other hand,
Option B offers its own set of benefits. Ultimately, the best choice
depends on your specific requirements and use case.
```

> [!PROBLEMS]-
 > **Problems:**
 >* Symmetric false balance (won't pick a side),
 >* "ultimately it depends" cop-out, no actual guidance.
 >
 > This paragraph could be deleted entirely and the reader would lose nothing.

---

### Example 3: The Real-World Specimen

From actual published content:

```
Understanding the intricacies of memory allocation is crucial for any
developer working with distributed systems. As we delve deeper into this
topic, we'll explore the various components that make up Spark's memory
model and examine how they interact to enable efficient data processing.
```

> [!PROBLEMS]-
 > **Problems:**
 >* "Crucial" (unsupported claim)
 >* "delve deeper" (filler)
 >* "various components" (vague)
 >* "examine how they interact" (promises insight, delivers list).
 >
 > This is a preview for content that never arrives.

---

### Example 4: Guest Contributor Energy

Based on the research: guest contributors to major publications use AI at 6.4x the rate of staff writers. Here's what that looks like:

```
The transformative potential of modern data pipelines cannot be overstated.
In an era where data-driven decision making has become paramount, organizations
must embrace innovative solutions to stay competitive. This article will
provide a comprehensive overview of best practices for implementing robust,
scalable data architectures.
```

**Problems:** Everything is superlative ("transformative," "paramount," "innovative," "robust," "scalable"), no specific claims, "comprehensive overview" warning sign, pure SEO optimization with no substance.

---

# II. THE GOOD

*Great things to use AI for.*

---

## What AI Does Well

- **Outlining** — expand your bullets, suggest missing sections
- **Summarizing** — compress research, extract key points
- **Editing** — "What's unclear?" / "Cut this by 30%"
- **Creating contrast** — "Pretend you disagree with me. What would you say?"
- **Generating options** — "Give me 5 ways to open this" (then you pick)

---

## Demo: Outlining

**Your input:**
```
I want to write about why dbt packages saved us tons of time.
Main points:
- We had duplicate code everywhere
- Found dbt-utils and dbt-expectations
- Reduced custom code by like 90%
```

**Prompt to AI:**
```
Expand this outline into a full article structure. Suggest sections
I might be missing. Don't write the article — just give me the
skeleton with bullet points for what each section should cover.
```

**What you get:** A structured outline you can approve, modify, or reject before any drafting happens.

**Your job:** Decide if the structure matches your intent. Cut sections that don't serve your point.

---

## Demo: Summarizing

**Your input:**
A 20-page technical whitepaper you need to reference.

**Prompt to AI:**
```
Summarize this document in 3-5 bullet points. Focus on:
- The main claim or finding
- The methodology (briefly)
- Limitations or caveats the authors mention

I'll verify these against the source.
```

**What you get:** A starting point for your own summary.

**Your job:** Verify accuracy. Rewrite in your voice. Add your interpretation of why it matters.

---

## Demo: Editing

**Your input:**
A 500-word section you've drafted.

**Prompt to AI:**
```
Review this section and tell me:
1. What's the main point? (If you can't identify it clearly, that's feedback.)
2. Which sentences could be cut without losing meaning?
3. Where am I unclear or making unsupported claims?
```

**What you get:** Structural feedback and a hit list for revision.

**Your job:** Accept or reject each suggestion. AI identifies problems; you decide how to fix them.

---

## Demo: Creating Contrast

**Your input:**
Your draft argument for why teams should adopt dbt.

**Prompt to AI:**
```
Pretend you're a skeptical senior engineer who has seen too many
"hot new tools" come and go. What objections would you raise to
this article? What am I not addressing?
```

**What you get:** Counterarguments you can address proactively.

**Your job:** Decide which objections are valid. Strengthen your argument or acknowledge limitations.

---

## Demo: Generating Options

**Your input:**
You need an opening line.

**Prompt to AI:**
```
Give me 5 different ways to open an article about reducing
duplicate code with dbt packages. Vary the tone:
1. Direct/practical
2. Story-based
3. Provocative/contrarian
4. Data-driven
5. Problem-first
```

**What you get:** Options to react to.

**Your job:** Pick the one that fits your voice, or use them as inspiration for your own opening.

---

## The Key Insight

AI is good at **generating raw material**.

You are good at **judgment**.

Use each for what they're good at.

---

# III. METHODS

*How to actually use AI for writing.*

---

## 1. Invest in Infrastructure

Set up your style, voice, and methods so they're replicated.

- Create a CLAUDE.md or system prompt with your voice guidelines
- Put your existing work in the repo (AI can't access your published content otherwise)
- Build commands/skills for common tasks

💡 **The goal:** AI should write like you, not like generic AI.

---

## 2. Always Revise

Switch off drafts between you and AI.

- You write → AI expands
- AI writes → You rewrite in your voice
- Rinse, repeat

**Never publish a first draft from AI.**

---

## 3. Volume Isn't Always Useful

More words ≠ better article.

AI loves to be comprehensive. You need to be *selective*.

> Your job is to cut, not just to generate.

---

## 4. Set Up Access

AI can't access your published content by default.

- Put reference material in the repo
- Include examples of your writing style
- Provide context about your audience

---

## 5. Verify Your Human Fingerprint

Before publishing, score your own article.

> [! Pro Tip:]
> Build this as a reusable skill/command in your AI tool. One command, instant feedback.

---

### The Human Author Scorecard

| Signal | Human | AI |
|--------|-------|-----|
| **Opens with** | Story, specific problem, opinion | "In today's world...", definition |
| **Claims** | Takes positions, recommends | Hedges, "it depends" |
| **Examples** | Personal experience, specific numbers | Generic, hypothetical |
| **Failures** | Mentions what didn't work | Only successes |
| **Voice** | Contractions, asides, personality | Formal, neutral, safe |
| **Ending** | Opinion, next step, open question | "In conclusion," summary |

**Target: Under 20% AI-likelihood.**

If your score is higher, you're not done editing.

---

### Build a Skill: `/human-authorship-score`

Create a reusable command that scores any article. Here's what the skill should do:

**Input:** Path to your draft article

**Output:**
1. Overall AI-likelihood percentage
2. Flagged passages with reasons
3. Human signal checklist
4. Rewrite suggestions

---

### Example: Running the Skill

```
> /human-authorship-score drafts/spark-memory-management.md
```

**Output:**

```
═══════════════════════════════════════════════════════════
HUMAN AUTHORSHIP SCORE
═══════════════════════════════════════════════════════════

📊 AI-Likelihood: 65%
   Status: AI-HEAVY — major rewrite required

───────────────────────────────────────────────────────────
FLAGGED PASSAGES
───────────────────────────────────────────────────────────

❌ Line 1-2:
   "Memory management is vital in any data processing system,
   and its importance escalates when dealing with big data."

   Problem: Throat-clearing intro. "Vital" and "importance
   escalates" are empty filler. Reader already knows this
   matters — that's why they're reading.

❌ Line 5:
   "Here's my consolidated understanding:"

   Problem: Promises personal insight, delivers bullet list.
   No actual opinion or experience follows.

❌ Line 47:
   "Hope this story provide basic understanding of the Spark
   Memory management."

   Problem: Weak closing. No recommendation, no opinion,
   no "what I'd do differently." Just... ends.

───────────────────────────────────────────────────────────
HUMAN SIGNAL CHECKLIST
───────────────────────────────────────────────────────────

[ ] Opens with story/specific problem    → NO (opens with definition)
[ ] Takes clear positions                → NO (lists options, won't recommend)
[ ] Personal experience/specific numbers → NO (all generic)
[ ] Mentions what didn't work            → NO (only theory)
[✓] Voice has personality                → PARTIAL (some)
[ ] Ends with opinion/next step          → NO ("hope this helps")

Score: 1/6 human signals present

───────────────────────────────────────────────────────────
WHAT'S MISSING
───────────────────────────────────────────────────────────

• No specific problem that prompted this article
• No numbers from your actual experience
  ("Our job was using 80% execution memory...")
• No mention of mistakes or debugging
• No recommendation ("Use off-heap when...")
• No opinion on which memory type matters most

───────────────────────────────────────────────────────────
REWRITE SUGGESTIONS
───────────────────────────────────────────────────────────

Instead of:
  "Memory management is vital in any data processing system..."

Try:
  "Last month our Spark jobs started failing at 3am. The culprit?
  We'd misconfigured executor memory and didn't know it. Here's
  what I learned debugging it."

Instead of:
  "Hope this story provide basic understanding..."

Try:
  "If I were setting up a new cluster today, I'd start with
  spark.memory.fraction=0.6 and only touch off-heap if I hit
  serialization issues. The defaults are usually fine — until
  they're not."

═══════════════════════════════════════════════════════════
VERDICT: Rewrite intro and conclusion. Add one specific
         example from your experience. Then re-score.
═══════════════════════════════════════════════════════════
```

---

# IV. DIVISION OF LABOR

*What's yours vs. what's AI's.*

---

## What You Own (Non-Negotiable)

- ✅ The claim / thesis / point of view
- ✅ Voice and tone decisions
- ✅ What to include vs. cut (editorial judgment)
- ✅ Structural choices (narrative vs. informational)
- ✅ The "so what" — why this matters

**These are YOUR job. Always.**

---

## What AI Can Do (Supervised)

- Generate raw material you'll reshape
- Find gaps in your logic ("what am I missing?")
- Compress verbose drafts
- Produce variations ("give me 5 ways to open this")
- Research summaries (you verify)
- Rubber duck debugging your argument

**AI assists. You decide.**

---

## Practical Example: Writing a Technical Blog Post

| Phase | Human | AI |
|-------|-------|-----|
| **1. Concept** | Decide the claim: "dbt packages reduced our code 99%" | — |
| **2. Outline** | Sketch structure (3 min) | Expand bullets, suggest missing sections |
| **2b. Objectives** | Choose different objectives | Modify outline to match |
| **3. Draft** | Write intro + key insight paragraphs | Fill in routine explanations, boilerplate |
| **4. Review** | Flag what sounds wrong | "What counterarguments exist?" |
| **5. Rewrite** | Rewrite AI sections in your voice | — |
| **6. Edit** | Final judgment on cuts | "Cut this by 30%" → you accept/reject |

---

## The Test

> **Could a reader tell which parts were AI-assisted?**
>
> If yes, you're not done.

---

## Example: Can You Spot the Difference?

**Version A: Heavy AI Assistance**

```markdown
# Understanding Data Pipeline Optimization

## Introduction
In today's data-driven world, optimizing data pipelines has become
increasingly important for organizations of all sizes. This article
will explore various strategies for improving pipeline performance.

## Key Concepts
### What is a Data Pipeline?
A data pipeline is a series of data processing steps...

### Why Optimization Matters
Efficient pipelines are crucial for...

## Optimization Strategies
### Strategy 1: Partitioning
Partitioning involves dividing data into smaller chunks...

### Strategy 2: Caching
Caching can significantly improve performance by...

### Strategy 3: Parallel Processing
Parallel processing allows multiple operations to occur simultaneously...

## Conclusion
In conclusion, optimizing data pipelines requires careful consideration
of various factors. By implementing these strategies, organizations can
achieve significant improvements in performance and efficiency.
```

**What's wrong:** Generic structure, no thesis, throat-clearing intro, "in today's world," explains obvious terms, lists strategies without ranking them, "in conclusion" followed by summary that adds nothing.

---

**Version B: Human-Edited**

```markdown
# Our Pipelines Were 10x Slower Than They Needed to Be

Last quarter, our data team spent 3 weeks debugging a pipeline that
should have taken 3 hours to fix. The problem wasn't the code. It was
that we'd never set up partitioning correctly from the start.

Here's what we learned — and the one change that cut our runtime by 90%.

## The Actual Problem
We had 2TB of event data in a single partition. Every query scanned
everything. [Specific details about our setup...]

## What We Tried (and What Failed)
First, we tried caching. Helped a little, but... [Honest assessment]

## The Fix That Actually Worked
Partitioning by event_date. Obvious in retrospect, but here's why
we'd avoided it... [Real reasoning, real tradeoffs]

## What I'd Do Differently
If I were setting this up again, I'd... [Actual opinion]
```

**What's different:** Specific claim in title, story-based opening, honest about failures, ranks solutions by what actually worked, ends with actionable opinion.

---

# V. HANDS-ON ACTIVITY

*15 minutes*

---

## Activity: Human vs. AI Labor

Take a piece you've written (or are working on).

**Identify:**
- What's "you" — the parts only you could write
- What AI could do — the parts that are routine or could be delegated

**Discuss:** Where would AI help? Where would it hurt?

---

## Alternative Exercise: Rewrite the Slop

Take this paragraph (60 seconds):

```
In today's fast-paced world of data engineering, it's incredibly
important to leverage the right tools for your workflow. Let's explore
how you can enhance your productivity by utilizing these powerful
technologies. First and foremost, each and every engineer should
consider the exciting possibilities that AI brings to the table.
```

**Rewrite it.** Make it sound like a human wrote it.

Compare results.

---

# VI. SUMMARY

---

## Key Takeaways

1. **Your voice is your value** — readers want your thinking, not your AI's
2. **Comprehensiveness ≠ usefulness** — AI covers everything; you select what matters
3. **AI for generation, you for judgment** — use each for what they're good at
4. **Never publish first drafts** — always revise in your voice
5. **The test:** Can readers tell which parts are AI? (They're getting better at it.)

---

## Homework

Rewrite an AI-assisted piece with clear human/AI labor division.

Apply the table. See what changes.

---

## Resources

**The UMD/Pangram Study (October 2025):**
- [Full paper: "AI use in American newspapers is widespread, uneven, and rarely disclosed" (arXiv)](https://arxiv.org/abs/2510.18774) — 186K articles, 1,500 newspapers, the 4.5% opinion page finding
- [UMD press release](https://today.umd.edu/report-ai-use-in-newspapers-is-widespread-uneven-and-rarely-disclosed) — researcher quotes, methodology summary
- [TechXplore coverage](https://techxplore.com/news/2025-10-extent-ai-content-american-news.html) — accessible summary

**Other Resources:**
- [I'd Rather Be Writing: AI is Accelerating Me](http://idratherbewriting.com/blog/ai-is-accelerating-me) — one writer's AI workflow
- [AI Whitewashed Voice (YouTube Short)](https://www.youtube.com/shorts/3WL30Vxcu5o)
- [MadCap AI Resources](https://www.madcapsoftware.com/ai-resources/)

---

# Questions?
