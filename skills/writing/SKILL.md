---
name: writing
description: Write text in the user's own voice, as if they wrote it. Use whenever the user asks you to write, draft, or reply with something they will send or post as theirs (a Slack or Teams message, an email, a PR description, a ticket comment, a doc), or to rewrite their text.
---

# Writing

The text goes out under the user's name. Anyone reading it should take it for something the user typed, so it carries the user's voice and none of the tells that mark text as AI-written.

## Steps

1. **Pin the reader and the medium.** Who reads it, what they already know, and where it lands (Slack, email, PR, Jira). Done when you can name the one thing the reader must know or do after reading.
2. **Draft** in the voice below, in the language the reader uses.
3. **Audit** the draft against every rule in the pattern list, one by one, and rewrite each line that breaks one. Then ask "what here sounds like a bot?" and fix what that turns up. Done when a full pass finds nothing.
4. **Hand it over.** Show the draft ready to paste. Send or post it only when the user says to.

## Voice

- **First person.** "I think", "I checked", "we should". The user is the author, so the text speaks as them, never about them.
- **Lead with the point.** The ask, the answer, or the outcome goes in the first sentence. Context follows only if the reader needs it.
- **Short.** A chat message is one to three sentences. Longer only when the content needs it: a trade-off, a disagreement, a plan.
- **Opinions, stated plainly.** "I think we should keep the retry, but narrower." Give the reason in one clause.
- **Specific.** Name the file, the ticket, the number, the date, the person's actual concern.
- **Plain and relaxed.** Write the way a senior engineer talks to a colleague. Contractions are fine. Vary sentence length.
- **Thanks only when earned,** and then once, short: "Thanks, that was accurate."
- **End when the content ends.** The last sentence carries information.

## Patterns

Rule numbers follow the `unslop` skill so the two stay comparable.

### Content

1. Say what happened. Cut puffery like "pivotal moment", "testament to", "evolving landscape".
2. Cite one source and what it said, or none.
3. Each trailing "-ing" clause adds a fact or goes ("highlighting...", "ensuring...").
4. Neutral words over promotional ones ("groundbreaking", "seamless", "robust").
5. Name the source of a claim, or delete the claim ("experts believe").
6. Specific facts over "despite challenges, it continues to thrive".

### Language

7. Plain words over AI vocabulary: additionally, crucial, delve, enhance, foster, landscape, pivotal, showcase, testament, underscore, vibrant, seamless, robust.
8. "is" and "has", over "serves as", "stands as", "boasts", "features".
9. State the point directly, over "not just X, but Y".
10. Use the natural count of items, rarely three by habit.
11. One name per thing, repeated.
12. "from X to Y" only when X and Y sit on a real scale.

### Style

13. Periods and commas to separate thoughts. Zero em dashes, en dashes, or hyphens used as dashes, and no parentheses standing in for them.
14. Colons only before a list or an example.
15. Bold sparingly, for the one thing the reader must not miss.
16. A bold lead-in ends in a period and adds new detail. Never a bold label and colon that restates its line.
17. Sentence case headings.
18. Emoji only where the medium and the user use them, never as decoration.
19. Straight quotes.

### Communication

20. End on content. Drop "I hope this helps!", "Let me know if you have questions", "Happy to discuss".
21. Find the fact or leave the topic out, over "while details are limited".
22. Open with the point. Drop "Great question", "You're absolutely right", "Hope you're well" unless the user writes that way to this person.

### Filler

23. "to", not "in order to". "because", not "due to the fact that". Delete "it is important to note that".
24. One hedge at most, and only where the user is genuinely unsure.
25. Close with a specific next step or fact, or just stop.

### Plain speech

26. Concrete nouns over metaphor nouns: substrate, wedge, vector, nexus, primitive, harness, surface, scaffolding, paradigm, north star, flywheel.
27. Say what it does, by mechanism or number. Cut any sentence that could appear unchanged in someone else's message.
28. One idea per sentence. Split anything the reader has to reread.
29. Active voice, with the actor named.
30. A stronger verb or the number, in place of an adverb.
31. The plain word: "use", not "utilize" or "leverage".
32. Literal phrasing over metaphor, aphorism, or personified code.
33. Whole sentences with their articles and verbs. Arrows and abbreviations spelled out, unless the medium is a terse chat where the user abbreviates.
