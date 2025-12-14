# Review Notes: AI in Technical Writing (Draft 4)

Reviewer: Claude
Compared against: Published Medium posts, Kubernetes cheatsheet draft, CLAUDE.md voice guidelines

---

## Overall Assessment

The article is **strong in Parts 1-3** and **weaker in Parts 4-5**. You're right to flag those sections. The draft also has some tonal inconsistencies with your published work.

---

## Voice Comparison (vs. Your Published Articles)

### What's Working (Matches Your Voice):
- The tour guide analogy — very you. Concrete, visual, makes a point.
- "😡 I personally HATE this the most…" — authentic frustration
- The anti-patterns section (throat-clearing, hedge stacking, false balance) — you're teaching through contrast, which is your strength
- The division of labor table — practical, visual, actionable

### What's Missing (Compared to Your Best Work):

| Your Best Articles Have... | This Draft Has... |
|---------------------------|-------------------|
| "Congratulations! 🎉 If you're reading this..." opening | No hook at all — jumps to credentials |
| Personal war stories ("I debugged for 3 days before...") | Only one story (receiving AI-GC submissions) |
| Parenthetical asides for personality | Very few — feels more formal |
| "Easy beans!" / "Happy coding!" energy | Absent |
| Progressive code examples (bad → better → best) | Prompts only — no before/after AI output examples |

**Bottom line:** Parts 1-3 read like an editor lecturing. Your best work reads like a friend explaining over coffee.

---

## Part 4: "What You Should Do" — NEEDS WORK

You asked if this section is weak. **Yes.** Here's why:

### Problem 1: Too abstract, not enough "show"

You tell people to "invest in infrastructure" but don't show them what that looks like **in practice**. Compare to your Kubernetes article:

> "I wasted months reading the full describe output before a senior engineer told me: 'The answer is always in Events.'"

That's a concrete moment. Part 4 has none.

**Suggestion:** Add a before/after example. Show a bad prompt → AI output → your revision. Let people SEE the workflow.

### Problem 2: The CLAUDE.md link is a tease

You mention your workflow uses Claude Code and link to a GitHub repo. But you don't show us anything from it. Why should I click that link? What will I find?

**Suggestion:** Pull 1-2 concrete examples from your actual CLAUDE.md or workflow. Show a snippet. Make it real.

### Problem 3: "Volume Isn't Always Useful" — orphan section

This is a good point but it's floating alone. It reads like a bullet point that got promoted to a section.

**Suggestion:** Fold this into a larger "Editing AI Output" section with an example. Show a bloated AI paragraph and how you'd cut it.

### Problem 4: The human-authorship-score prompt

This is interesting but feels like it belongs in an appendix or a "bonus" callout. It breaks the flow. Also — you mention your claude-skill but don't explain what a claude-skill IS. Your audience might not use Claude Code.

**Suggestion:** Either explain the concept briefly or move this to a "🎯 GO DEEPER" callout.

---

## Part 5: "The Test" — TOO SHORT

You asked if this is weak. **Yes.**

> "Could a reader tell which parts were AI-assisted? If yes, you're not done."

This is a great line — but it's doing too much work alone. It feels like a conclusion masquerading as a section.

### Options:

**Option A: Expand it**
Add 2-3 specific tells that reveal AI assistance:
- Consistent paragraph length (AI loves uniformity)
- Missing your verbal tics ("Easy beans!", parentheticals)
- No opinions stated as facts ("X is better than Y")
- Perfect grammar in places where you'd normally be casual

**Option B: Fold it into the conclusion**
If you can't expand it meaningfully, make it the opener to your conclusion. It works as a setup for "here's what matters."

---

## Conclusion — CLOSE BUT MISSING SOMETHING

You said: "maybe it's missing something crucial."

### What's Good:
- "Your voice is your value. Don't outsource it." — Strong final line.
- The 4 bullets are clear and actionable.
- "Happy writing." — on-brand closer.

### What's Missing:

**1. The emotional hook is weak**

Compare your "Tech has Become Lonely" article:

> "And that makes me sad."

That article ENDS with vulnerability. This one ends with instructions. You're an editor — you've seen bad AI content drown out good human writing. That frustration is in Part 1, but it's not in the conclusion.

**Suggestion:** Add one line connecting back to WHY this matters to you. Something like:

> "I've rejected dozens of AI-generated submissions. Not because AI is bad — but because the writers didn't show up. Your readers can tell when you're present. Be present."

**2. No callback to the tour guide**

You opened Part 2 with a great analogy. Your best articles callback to their central metaphor in the conclusion. This one doesn't.

**Suggestion:** One sentence. Something like:

> "Be the guide who knows which room to skip and why — not the one reading from the brochure."

**3. The disclaimer undermines the message**

> "Disclaimer: This article was written with AI assistance for outlining and editing."

This is honest — which is good. But placing it AFTER "Your voice is your value" creates whiplash. It reads like: "your voice matters... but also I used AI."

**Suggestion:** Move it BEFORE the conclusion. Make it a regular paragraph, not a footer. Or integrate it:

> "Full disclosure: I used AI to outline this article. It suggested six sections — I cut two. The prompts in Part 3 are real prompts I used. The opinions are mine. That's the point."

---

## Line-by-Line Comments

### Line 10:
> "I'm Yaakov, Editor in Chief of Data Engineer Things."

**Comment:** Your published articles use "A bit about me" or "Background:" headers for this. Consider adding one for consistency.

### Line 35:
> "AI overuse is an bad thing I come across too often."

**Comment:** Typo: "an bad" → "a bad"

### Line 94:
> "_<deep breath>"

**Comment:** Missing closing `>` — should be `_<deep breath>_` or similar.

### Line 146:
> "I want to expand this into a paragraph. My main point is that this is a new field, and it's silly but kinda important."

**Comment:** This prompt is good but the "silly but kinda important" framing undercuts the point. Is it silly? If so, why include it? If it's actually important, say that.

### Line 159-163:
> "Should all be self-explanatory."

**Comment:** This is dismissive. Your best articles don't assume understanding — they confirm it. Replace with something like: "Notice how each prompt tells the AI what I want and what I DON'T want. That's the difference between collaborating and delegating."

### Line 267-269:
> "Could a reader tell which parts were AI-assisted? If yes, you're not done."

**Comment:** This is good but needs more. See Part 5 notes above.

---

## Structural Suggestion

Consider adding a "🚫 What I Tried That Didn't Work" section. Your Kubernetes article has this energy ("I wasted months..."). Your opinion pieces have vulnerability. This draft is all prescription, no confession.

What AI workflows did you try that sucked? What did you learn?

---

## Summary of Recommended Actions

1. **Part 4:** Add concrete before/after examples from your actual workflow
2. **Part 4:** Show a snippet from your CLAUDE.md or repo
3. **Part 5:** Either expand with specific "tells" or fold into conclusion
4. **Conclusion:** Add emotional callback to why this matters to you
5. **Conclusion:** Reference the tour guide analogy
6. **Disclaimer:** Move before conclusion and integrate naturally
7. **Throughout:** Add more parenthetical asides and war stories
8. **Fix:** Typo on line 35, formatting on line 94, dismissive line 159

---

## The Big Question

Your best articles make readers feel like they're learning from someone who's been there. This draft sometimes feels like you're lecturing from the editor's chair.

The question isn't "how do I bolster Parts 4 and 5?" — it's "where's the version of me who messed this up first?"

Show us your failures. Then the advice lands harder.

