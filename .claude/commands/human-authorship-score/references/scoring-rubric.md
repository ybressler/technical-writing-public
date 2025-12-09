# Scoring Rubric

Detailed criteria for each component score.

## Stance (Default 25%)

How strongly does the writer take positions?

| Score | Criteria |
|-------|----------|
| 90-100 | Clear thesis, specific recommendations, defends positions, willing to say "this is wrong" |
| 70-89 | Takes positions but hedges occasionally, makes some recommendations |
| 50-69 | Positions present but softened, frequent "it depends," limited recommendations |
| 30-49 | Mostly descriptive, avoids commitment, symmetric balance on everything |
| 0-29 | No positions, pure hedge, "there are many perspectives to consider" |

**Key signals:**
- High: "Use X, not Y" / "This approach is wrong because..." / "I recommend..."
- Low: "It depends on your situation" / "There are trade-offs to consider" / "Some prefer X while others prefer Y"

## Specificity (Default 25%)

Does the writer use concrete, personal, verifiable details?

| Score | Criteria |
|-------|----------|
| 90-100 | Personal experience with specifics, real numbers, named failures, unique examples |
| 70-89 | Some personal experience, occasional specific numbers, one or two concrete examples |
| 50-69 | Generic examples, hypothetical scenarios, round numbers, could be anyone's article |
| 30-49 | Abstract throughout, no personal reference, "imagine a scenario where..." |
| 0-29 | Pure abstraction, no examples, or only obvious/stock examples |

**Key signals:**
- High: "We reduced latency from 340ms to 12ms" / "I tried X in 2019 and it failed because..."
- Low: "This can significantly improve performance" / "Consider a typical use case..."

## Voice (Default 20%)

Is there a distinctive human author present?

| Score | Criteria |
|-------|----------|
| 90-100 | Strong personality, natural contractions, asides, humor or edge, memorable phrasing |
| 70-89 | Some personality visible, occasional contractions, mostly consistent tone |
| 50-69 | Neutral but not robotic, could be any competent writer |
| 30-49 | Flat, formal, interchangeable with other articles on topic |
| 0-29 | Robotic, sycophantic, false enthusiasm, hedge stacking, "exciting opportunity" |

**Key signals:**
- High: Asides in parentheses, contractions ("don't" not "do not"), specific word choices, humor
- Low: "It's important to note" / "Let's dive in" / "That's a great question"

## Opening (Default 15%)

Does the opening hook with something human?

| Score | Criteria |
|-------|----------|
| 90-100 | Starts with specific story, surprising claim, or direct opinion |
| 70-89 | Starts with problem or context, gets to point within first paragraph |
| 50-69 | Mild throat-clearing but recovers quickly |
| 30-49 | Definition lead, "In today's world...", preview of article structure |
| 0-29 | "X is defined as..." / "This article will explore..." / Multiple paragraphs before substance |

**Key signals:**
- High: "Last month our pipeline broke at 3am and I learned..." / "Most advice about X is wrong."
- Low: "In today's rapidly evolving landscape..." / "Understanding X is crucial for any developer..."

## Closing (Default 15%)

Does the ending offer something beyond summary?

| Score | Criteria |
|-------|----------|
| 90-100 | Ends with opinion, specific recommendation, open question, or "If I were starting over..." |
| 70-89 | Some opinion or forward-looking thought, minimal summary |
| 50-69 | Brief summary but adds something new |
| 30-49 | "In conclusion" + summary of article |
| 0-29 | Formulaic close, "By implementing these best practices...", generic call to action |

**Key signals:**
- High: "If you take one thing from this: do X" / "I'm still not sure about Y—what do you think?"
- Low: "In conclusion, we have explored..." / "By following these steps, you can..."

## Genre Adjustments

Apply these weight modifications:

| Genre | Stance | Specificity | Voice | Opening | Closing |
|-------|--------|-------------|-------|---------|---------|
| Essay/Opinion | 25% | 25% | 20% | 15% | 15% |
| Tutorial | 20% | 30% | 15% | 15% | 20% |
| Reference | 15% | 35% | 10% | 20% | 20% |
| Narrative | 20% | 25% | 25% | 20% | 10% |
| News/Report | 20% | 35% | 10% | 20% | 15% |

## Edge Cases

**Technical reference docs:** Expect lower Voice scores. Focus on Specificity and clear Opening. Score 60+ is acceptable.

**Edited AI content:** May score 50-70. Look for inconsistency—human sections vs. AI sections. Flag the contrast.

**Bland human writers:** Some humans write without personality. Confidence should be lower (50-70%) when Voice is low but other signals are ambiguous.

**Non-native English:** Don't penalize grammar. Focus on whether claims, specifics, and personality are present regardless of fluency.
