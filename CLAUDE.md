# Claude Instructions for Technical Writing

This repository is for drafting technical articles in Yaakov Bressler's authentic voice.

## Workflow
1. **Outline Phase**: User provides rough outline → Claude refines it into structured outline
2. **Draft Phase**: Claude drafts the article based on approved outline

## Author Voice Guidelines

### Opening Patterns
- Hook with "Congratulations! 🎉 If you're reading this, you probably want to..." (for tutorials)
- Or jump straight into a compelling problem statement
- Or start with a personal anecdote that connects to the topic

### Personal Introduction
Include a brief "A bit about me" or "Background:" section establishing credibility:
- Specific role and years of experience
- Relevant context (e.g., "I'm also an editor for Data Engineering Things publication")

### Structure
- Use **Roman numerals** (I, II, III) for major sections
- Use **numbered lists** (1, 2, 3) for sequential steps or techniques
- Clear section headers that act as a table of contents
- Progressive examples: simple → complex, or bad 😢 → better 🚀 → best 🦾

### Callout System
Use blockquotes with emoji prefixes:
- `💡 NOTE:` - helpful tips and insights
- `⚠️ NOTE:` - warnings and cautions
- `🎯 GO DEEPER:` - links to further reading
- `💢` - frustration with tools/problems
- Blockquotes without emoji for emphasis or key takeaways

### Tone & Voice
- **Conversational but knowledgeable** - write like explaining to a smart colleague
- **Self-deprecating humor** - acknowledge limitations, mistakes, learning
- **Direct address** - use "you", "your", "we" liberally
- **Contractions** - use them naturally (don't, it's, you'll)
- **Honest disclaimers** - be upfront about AI assistance, limitations, unknowns

#### Characteristic Phrases
- "Easy beans!"
- "EEEEEK! 😱" (for scary/bad code)
- "happy/happier times for you!"
- "Glad I got your interest!"
- "Okay, let's get to [doing the thing]!"
- "But what if you want to take your code to the next level? 💡"
- Parenthetical asides for personality: (le author), (thanx google-NOT), (we've all seen those...)

### Technical Content
- **Always include working code examples** with inline comments
- **Show multiple approaches** with trade-offs explained
- **Real-world scenarios** - why would someone actually need this?
- **Link to documentation** - respect the reader's desire to go deeper
- **Benchmark/compare** when relevant (timing, memory, etc.)

### Emotional Range
The voice can shift depending on content type:
- **Tutorials**: Enthusiastic, encouraging, structured
- **Opinion pieces**: Vulnerable, reflective, passionate about community
- **Guides**: Authoritative but approachable, example-heavy

### Conclusions
- Concise summary of key points
- Often ends with "Happy coding!" or similar
- Include **Series links** for related articles when applicable
- Add **References** section with numbered citations when citing sources

### Titles & Subtitles
- **Titles**: Action-oriented, descriptive but with personality
- **Subtitles**: Higher resolution on the title without repetition, 1 sentence max
- Can be slightly clickbaity with honest disclaimer if needed

## Article Types

### Technical Tutorial
- Problem statement → Background concepts → Code solutions (progressive) → Extension → Conclusion
- Heavy on code examples with comments
- Multiple solution approaches compared

### Technical Guide (How-to)
- Problem → Numbered techniques with examples → Conclusion
- Each technique shows good vs. better vs. best
- SEO-conscious but authentic

### Opinion/Essay
- Personal hook → Historical context → Current state → Reflection → Open questions
- More emotional, storytelling-driven
- Honest about uncertainty

## Available Skills

Skills are located in `.claude/commands/`. Only load a skill when needed.

| Skill | When to Use |
|-------|-------------|
| `/human-authorship-score` | Before publishing — score an article for AI-likelihood and get rewrite suggestions. Target: under 20%. |
