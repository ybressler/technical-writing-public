# AI in Technical Writing
## Good ways to use AI and bad ways to use AI.

---

# I. THE BAD

*Things to avoid when using AI for writing.*

---

## The "Whitewashed Voice"

AI writing sounds like... AI writing.

- Formulaic and robotic
- Neurotically positive — everything is "great," "exciting," "important"
- Hedged to death — "It's important to note that it may be worth considering..."
- Written for beginners (even when it shouldn't be)

**The result?** Bloat. AI Slop. 🤮

---

## Voice Problems

| Pattern                   | Example                              | Why it fails                             |
| ------------------------- | ------------------------------------ | ---------------------------------------- |
| **Sycophantic openers**   | "That's a great question!"           | Reader isn't asking you to validate them |
| **Hedge stacking**        | "It may be worth considering..."     | Says nothing, burns trust                |
| **Neurotically positive** | Everything is "exciting," "powerful" | No credibility, no contrast              |
| **False enthusiasm**      | "Let's dive in!"                     | Filler energy, no substance              |

---

## Structure Problems

| Pattern | Example | Why it fails |
|---------|---------|--------------|
| **Throat-clearing intros** | "In today's fast-paced world of data engineering..." | Delays the point, reader skips anyway |
| **Everything for beginners** | Explaining what an API is in an advanced post | Wrong audience, bloat |
| **Compulsive completeness** | Listing every edge case | Buries signal in noise |
| **Symmetric false balance** | "On one hand... on the other... it depends" | Avoids taking a position |

---

## Detail Problems

| Pattern | Example | Why it fails |
|---------|---------|--------------|
| **Redundant pairs** | "each and every," "first and foremost" | Empty calories |
| **Explaining the obvious** | "This is important because it matters" | Circular, adds nothing |
| **Defensive citations** | Supporting claims no one disputes | Wastes reader attention |
| **List bloat** | 10 items when 3 make the point | Dilutes impact |

---

## The Meta-Problem

> AI writes to **avoid being wrong**.
>
> You should write to **be useful**.

AI hedges because confidence is risky.

Good technical writing takes positions.

---

## Why Does This Matter?

**The real question:**

> People can talk to AI themselves. Why should they read *your* conversation with it?

They want your thinking. Your voice. That's the value.

---

## 🔴 Exercise: Spot the Slop

*Show a paragraph written with AI assistance. Redline the problems together.*

```
In today's rapidly evolving landscape of data engineering, it's important
to note that leveraging AI tools can be a powerful way to enhance your
workflow. Let's dive in and explore how you can use these exciting
technologies to boost your productivity. First and foremost, it's worth
considering that each and every data engineer should...
```

**What's wrong here?** _(Let participants call it out)_

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

1. **AI writes to avoid being wrong. You write to be useful.**
2. **Your voice is the value** — readers want your thinking, not your AI's
3. **AI for generation, you for judgment**
4. **Never publish first drafts** — always revise
5. **The test:** Can readers tell which parts are AI? If yes, keep editing.

---

## Homework

Rewrite an AI-assisted piece with clear human/AI labor division.

Apply the table. See what changes.

---

## Resources

- [I'd Rather Be Writing: AI is Accelerating Me](http://idratherbewriting.com/blog/ai-is-accelerating-me) — helpful guide on one writer's AI workflow
- [AI Whitewashed Voice (YouTube Short)](https://www.youtube.com/shorts/3WL30Vxcu5o)
- [MadCap AI Resources](https://www.madcapsoftware.com/ai-resources/)

---

# Questions?
