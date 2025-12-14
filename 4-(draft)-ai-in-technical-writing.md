
### (How to Use) AI in Technical Writing

#### Without losing your voice and sounding like a robot.

![image](https://cdn-images1.medium.com/max/1440/1*YXCAAeyj22tYa0DnFOD4Ow.jpeg)

#### Introduction:

I’m Yaakov, Editor in Chief of [Data Engineer Things](https://www.dataengineerthings.org/). Our publication receives a lot of AI generated content (AI-GC). This content is bad because it is lazy, robotic, and annoying. I hate pure AI-GC. _(And remove those authors from our publication…)_

And yet… I use AI for everything. Including writing this article! So let’s figure out how to use AI in technical writing, without being awful.

> _💡_ My goal isn’t to ban technology, but to fix how we use AI in technical writing.

### PART 1. AI Content IS BAD

> In case you need someone to tell you… 

People can tell when you’ve let AI do all the writing. And they [hate](https://raptive.com/blog/the-ai-stink-is-real-and-its-costing-brands/) it.

#### **People can talk to AI themselves.**

**_Why should they read YOUR conversation with it?_**

Your value as a writer isn’t your ability to produce words (or hit SEO targets). It’s your voice. Your experience in the world (as a human), and the judgement and biases that come with that.

AI has no judgment. It has no point of view. It just… produces words.

---

### PART 2: What AI Writing Sounds Like (Don’t Do This)

AI overuse is an bad thing I come across too often.

Let me show you what I mean.

#### The Tour Guide Analogy

Imagine you’re at a museum and you hire a tour guide.

![](https://cdn-images-1.medium.com/max/1440/1*cMKrhr60JiK5Ze3dHdD_ww.jpeg)

![](https://cdn-images-1.medium.com/max/720/1*eQKQQ6OhxyWjnM_aYtGL_g.jpeg)

#### Bad tour guide (AI voice):

> “Welcome! This is going to be an exciting journey! The museum is a truly remarkable institution with many important exhibits. Let’s explore the fascinating world of art together!”

#### Good tour guide (human voice):

> “Skip the first three rooms — they’re renovation leftovers. But room 4 has a Vermeer they acquired last year that nobody knows about. I’ll show you the angle where you can see his signature hidden in the tablecloth.”

The bad guide tells you everything is important. The good guide tells you what **actually** matters.

---

### AI (Anti)Patterns

Here’s what (bad) AI writing actually looks like. Learn to spot these:

#### 1. Throat-Clearing Intros

> In today’s fast-paced world of software development, efficient data processing has become more critical than ever. As organizations increasingly rely on data-driven decision making, understanding the tools and techniques available has never been more important.

This is the written equivalent of someone saying “um” for 30 seconds. The reader already knows data is important — that’s why they clicked on your article. Start with your actual point.

#### 2. Hedge Stacking

> It’s important to note that while there may be some potential benefits to this approach, it’s worth considering that results can vary depending on your specific use case.

Count the hedges: “important to note,” “may be,” “potential,” “worth considering,” “can vary.” This sentence commits to nothing. If you’re not willing to say something definite, why are you writing?

#### 3. Neurotically Positive

> In today’s rapidly evolving landscape of data engineering, it’s incredibly exciting to explore the powerful possibilities that modern tools bring to your workflow.

Count the empty superlatives: exciting, powerful, game-changing, transformative. None of these words communicate anything specific. This is hype without substance.

> _😡_ I personally HATE this the most… Stop being so… happy!

#### 4. False Balance

> There are several approaches to handling this problem. On one hand, you could use Option A, which has certain advantages. On the other hand, Option B offers its own set of benefits. Ultimately, the best choice depends on your specific requirements.

This paragraph could be deleted entirely and the reader would lose nothing. AI won’t pick a side because it has no opinion.

If you can’t defend a position, don’t say anything!

---

### PART 3: AI IS GOOD

_<deep breath>

Let’s talk about how AI can actually be helpful for technical writing.

- Outlining
- Editing
- Creating Contrast
- Generating Options
- Continuing your train of thought.

---

_Here’s what each looks like (as a prompt):_

#### Outlining:

I want to write about why dbt packages saved us tons of time.  
Main points:  
- We had duplicate code everywhere  
- Found dbt-utils and dbt-expectations  
- Reduced custom code by like 90%  
  
  
Expand this outline into a full article structure. Suggest sections  
I might be missing. Don't write the article — just give me the  
skeleton with bullet points for what each section should cover.

#### Editing:

Review this section and tell me:  
1. What's the main point? (If you can't identify it clearly, that's feedback.)  
2. Which sentences could be cut without losing meaning?  
3. Where am I unclear or making unsupported claims?

#### Creating Contrast:

Pretend you're a Staff+ Software Engineer who has seen too many  
"hot new tools" come and go. You love to be right - and often are!  
What objections would you raise to this article? What am I not addressing?

#### Generating Options:

Give me 5 different ways to open an article about reducing  
duplicate code with dbt packages. Vary the tone:  
1. Direct/practical  
2. Story-based  
3. Provocative/contrarian  
4. Data-driven  
5. Problem-first

#### Continuing Train of Thought:

I started writing the folllowing:  
  
> An emerging field of academic research has emerged, studying how AI Slop  
> works, and why people hate it.  
  
  
I want to expand this into a paragraph. My main point is that  
this is a new field, and it's silly but kinda important. Go and  
write it in my voice - if you're not sure about something, pause and  
ask me fo clarity and I will provide it. 

---

Should all be self-explanatory.

![](https://cdn-images-1.medium.com/max/1440/0*lVckttSMFDXcQXbk.jpg)

AI is a very useful tool. But it is not the “author.” I am driving the conversation.

  

### PART 4: WHAT YOU SHOULD DO

**TLDR:** Invest in infrastructure.

_Here’s my actual workflow, using_ [_Claude Code_](https://claude.com/product/claude-code)_._

You can see the work + infrastructure + iterations that went into writing this article here: [https://github.com/ybressler/technical-writing-public/tree/main](https://github.com/ybressler/technical-writing-public/tree/main)

---

#### 1. Invest in Infrastructure

Set up your style, voice, and methods so they’re replicated.

- Create a `CLAUDE.md` or system prompt with your voice guidelines
- Put your existing work somewhere the AI can see it (it can’t read your published Medium posts).
- Build reusable prompts for common tasks

> **_💡_ The goal:** AI should write like **you**, not like generic AI.

---

#### 2. Always Revise

Switch off drafts between you and AI:

- You write → AI expands
- AI writes → You rewrite in your voice
- Rinse, repeat

> **_🚫_** Never publish a first draft from AI.

> **_🚫_** Never publish a first draft period.

---

#### 3. Volume Isn’t Always Useful

AI loves to be comprehensive. You need to be **_selective_**.

More words ≠ better article. Your job is to cut, not just to generate.

---

#### 4. Verify Your Human Fingerprint

Before publishing, check to see the “human author score” of your article. You can use a prompt like so:

Review the following article and give it a score of  
"human authorship."  
  
- 100 means it is very human (and good).  
- 0 means it is straight up AI slop.  
  
Then I want a score for certain components. (You will need to   
come up with 4-5 subcomponents to give a rating for.) Overall,  
these components should form the larger overall score.

I personally use a [claude-skill](https://www.claude.com/blog/skills) to rate articles:  
`[human-authorship-score/SKILL.md](https://github.com/ybressler/technical-writing-public/blob/main/.claude/commands/human-authorship-score/SKILL.md)` (feel free to copy it and use).

---

#### 5. Division of Labor

Here’s the split:

**What You Own (Non-Negotiable):**

- The claim / thesis / point of view
- Voice and tone decisions
- What to include vs. cut (editorial judgment)
- Structural choices
- The “so what” — why this matters

**What AI Can Do (Supervised):**

- Generate raw material you’ll reshape
- Find gaps in your logic
- Compress verbose drafts
- Produce variations
- Research summaries (you verify)

**TLDR: AI assists. You decide.**

PHASE    | YOU (The Brain)         | AI (The Hands)  
---------+-------------------------+----------------------  
Concept  | Decide the claim        | —  
Outline  | Sketch structure (3m)   | Expand/Fill gaps  
Draft    | Intro + Key insights    | Routine explanations  
Review   | Flag odd phrasing       | Gen. counterarguments  
Rewrite  | Rewrite AI sections     | —  
Edit     | Final judgment          | Suggest cuts

---

### Part 5: The Test

Here’s how you know you’re done:

#### **_Could a reader tell which parts were AI-assisted?_**

If yes, you’re not done.

---

### Conclusion

If you only read 1 part of this article, read this.

1. **Use AI for the scaffolding, not the substance:** Outlines, summaries, options.
2. **Your opinion is the product:** If you don’t have one, you’re not ready to write the thing.
3. **When in doubt, cut:** AI adds junk. Good writing is intentional and focused.
4. **The goal isn’t to produce content:** It’s to help someone who reads it. Keep that person in your head the whole time.

Your voice is your value. Don’t outsource it.

Happy writing.

  

> **_Disclaimer:_** This article was written with AI assistance for outlining and editing. The opinions, examples, and bad jokes are mine.

---

#### Further Reading:

- MEASURING AI “SLOP” IN TEXT: [https://arxiv.org/pdf/2509.19163](https://arxiv.org/pdf/2509.19163)?
- When AI turns culture into slop: [https://link.springer.com/content/pdf/10.1007/s00146-025-02630-1.pdf](https://link.springer.com/content/pdf/10.1007/s00146-025-02630-1.pdf)