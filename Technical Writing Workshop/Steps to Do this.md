1. Write outline
2. Have claude add sections to the outline:
	1. What are some AI behaviors to avoid?
3. Finish outline - have AI deduce my objective + my reader's objective
   `Based on this outline, deduce my motive/objective. And what would the objective be of my reader?`
4. Modify outline as needed


# Objectives:

### **Your objective (writer):**
Help writers use AI without becoming invisible. Protect what makes their writing worth reading—their thinking, their voice, their judgment.

### Secondary:
Give writers an AI workflow so they're not guessing.

### **Reader's objective:** 
"I want to use AI to write faster, but I don't want my writing to sound like everyone else's. What's the line?"

### TENSION:
> *"Am I already doing this wrong? How do I know?"*


## Feedback for AI
AI wrote this in my 1st draft:

```text
## The Meta-Problem

> AI writes to **avoid being wrong**.
>
> You should write to **be useful**.

AI hedges because confidence is risky.

Good technical writing takes positions.
```

Frankly, I don't buy this. This is an unsupported claim. BAD. (Use this as an example for what to avoid - sycophantic language and retort based on symmetrical argument, rather than intent and purpose.



---

Great work. Note, I moved the draft to "Technical Writing Workshop" directory. I want next to create a 2nd draft, and I will give you detailed feedback on things I want  changed and/or enhanced:

  1. For the section "## The "Whitewashed Voice" I want examples. Not in chart form. Give the example a title as a descriptor, then the example, then commentary on what's   wrong. Here's an example of an example:

  ### Example: Formulaic and robotic
  > Memory management is vital in any data processing system, and its importance escalates when dealing with big data. In Apache Spark, grasping the fundamentals of in-memory
  processing is key to optimizing performance. Here’s my consolidated understanding:
  >
  > There are different level of memory management in Spark
  > On-Heap Memory
  > Overhead memory
  > Off -Heap Memory

  Formulaic and bad! - provide details why, prove the point

  2. Voice Problems
  Give an analogy (in my slideshow, this will be a new slide, to lighten the content make it more fun). Should be an addition. What you have is good, I want to add to it.

  3.  Structure Problems
  I want something more significant that sentence level feedback. Here is an article that clearly abuses AI:
  https://medium.com/@vtrkayalrajan/spark-memory-management-and-its-types-425af52d7c15 Show why and how from structure
  (If you cannot access it, ask me and I'll paste the content)

  4. " AI writes to **avoid being wrong**."
  Frankly, I don't buy this. This is an unsupported claim. BAD. (Use this as an example for what to avoid - sycophantic language and retory based on symetrical argument,
  rather than intent and purpose."

  5. "People can talk to AI themselves. Why should they read *your* conversation with it?"
  Enhance this section. Give more support to it. (Ideally, y9ou have proof)

  6. Exercise: Spot the Slop
  Excelllent! Love this! Give more examples! Ideally one or 2 from well known publications (ex: Maybe the NYT or WSJ wrote about something related to this not too long ago?)

  7. For the details in "What AI Does Well"
  I want a prompt you can use for each. So maybe create a section titled "Demo:" and give the steps you might use with an AI to co-work, on the things it does well.

  8. "**Could a reader tell which parts were AI-assisted?**"
  Give an outline that is written with heavy AI assistance, then enhance it. let's see if we can see.

### Create a Claude Code skill
```text
I want to build a skill in claude code to review an article and give it a score of "human authorship." A 100 means it is very human (and good). A 0 means it is straight up AI slop.

Give a subscore of confidence (also 0-100%) it is okay to not be able to tell.

Then I want a score for certain components. (You will need to come up with 4-5 subcomponents to give a rating for.) Overall, these components should form the larger overall score.

I want your idea for how to create this score. And we will go back and forth until we feel confident with the skill, then I will create the skill for claude code.
```
