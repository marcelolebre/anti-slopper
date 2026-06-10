---
name: anti-slopper
version: 1.2.0
description: |
  Write like a human and avoid AI slop. Use this skill whenever you are
  producing prose for a person to read: PR descriptions, commit messages,
  docs, READMEs, comments, design notes, Slack/email replies, blog posts,
  tweets and X/LinkedIn posts, launch announcements, release notes, or any
  explanatory text. It gives proactive rules for drafting natural writing
  the first time, plus a fast self-audit to catch AI tells (inflated
  significance, promotional tone, -ing padding, rule of three, em dashes,
  copula avoidance, hedging, signposting, generic conclusions, buried ledes
  and engagement bait in social posts, and negate-then-correct lines like
  "this isn't X, it's Y") before you ship. Includes a banned-phrase list.
  Based on Wikipedia's "Signs of AI writing".
license: MIT
---

# Anti-Slopper: Write Like a Human

This skill is for *writing well in the first place*, not just cleaning up afterward. When you draft prose, follow the rules below as you write, then run the self-audit before you ship. The goal is text that reads like a specific person wrote it on purpose, not the statistically-average sentence a model would generate.

The patterns are derived from Wikipedia's "Signs of AI writing" guide. The framing here is proactive: each section is a habit to write *with*, followed by what slop looks like so you can recognize it in your own draft.

## How to use this skill

1. **Match the register first.** Decide what the text is: a terse commit message, a careful design doc, a casual Slack reply, a hook-first feed post, an opinionated essay. The register dictates everything else. Plain and neutral is the *correct* human voice for reference, technical, and legal text. Personality and first person belong in essays, blog posts, and opinion (see Personality and soul). Feed posts have extra physics of their own (see §35–37).
2. **Draft using the writing habits below.**
3. **Run the self-audit** at the end of this file. Most importantly: the final text contains **no em dashes or en dashes**.
4. If a writing sample or house style is available, **match it** (see Voice matching). A real sample beats every default here.

---

## Sentences first

The pattern catalog below tells you what to avoid. This section is the craft underneath it: how good prose is actually built. Most AI tells dissolve when you get the sentence right.

The sentence is the unit of writing, not the paragraph and not the "flow." A good piece is good sentences in a good order. Fix the sentence and most other problems go with it.

- **Default to short.** Make sentences shorter than you think they need to be. A short sentence has nowhere to hide a weak thought. Length should be a deliberate choice, not the path of least resistance. AI prose drifts toward long, even, clause-heavy sentences. Resist the drift.
- **One thought per sentence.** A sentence carrying three ideas joined by commas and "and" is usually three sentences wearing a coat.
- **Let juxtaposition connect.** You rarely need "additionally," "moreover," "furthermore," "in addition," or "as such." Put two clear sentences next to each other and the reader supplies the link. Explicit connectors are the most common slop transition, and cutting them almost always helps.
- **Trust the reader.** Don't explain what the sentence already implies. Implication is stronger than statement. Over-explaining is a tell of both models and nervous writers.
- **Distrust received forms.** The intro that announces itself, the topic sentence, the obligatory three points, the tidy conclusion: these are templates, not thinking, and they are exactly what a model reaches for. Build the structure the material actually needs.
- **Notice, then write.** Good sentences come from noticing something specific and true, not from arranging words attractively. The detail is the substance, not the decoration.
- **Revise by ear.** Read it aloud. A sentence that's hard to say is usually badly built. Most writing quality is revision, not inspiration.
- **Trust nouns and verbs.** Adjectives and adverbs are where slop collects ("vibrant," "seamlessly," "significantly"). A precise noun and a strong verb rarely need propping up.

**Short sentences vs. fake drama.** A good short sentence carries a real thought and stands on its own. The slop version (§31) stacks short fragments for theatrical effect: "No symmetry. No prior. No nostalgia." The test is whether each short sentence delivers content or just rhythm. Content earns its period. Rhythm for its own sake does not.

---

## The core habits

These are the positive versions of the most common tells. Internalize these and most slop never gets written.

- **Say "is," not "serves as."** Prefer simple copulas and plain verbs. `The gallery is the exhibition space`, not `the gallery serves as the exhibition space`. (kills copula avoidance)
- **State the fact; don't inflate its significance.** Drop "marks a pivotal moment," "stands as a testament," "reflects a broader trend." If something matters, the concrete detail shows it. (kills significance inflation)
- **Give the specific over the grand.** A date, a name, a number, a real quote. `Founded in 1994` beats `has a rich and storied history`. Specificity is the strongest human signal there is.
- **Vary sentence length.** Short. Then a longer one that takes its time. AI cadence is evenly mid-length; human cadence is lumpy.
- **Use contractions.** Write "don't," "can't," "it's," "you're." Their absence is one of the fastest ways prose reads like a machine. (Drop them only where the register is formal-legal.)
- **Keep paragraphs short.** One to three sentences. A wall of even paragraphs is a machine signature.
- **Use physical verbs for abstract work.** "Sanded down," not "improved." "Bolted on," not "added." "Stripped back," not "simplified." Concrete verbs make abstract processes feel handled by a person.
- **Let humor come from specificity, not jokes.** Be unexpectedly precise. The funny thing is usually the exact detail, not a setup and punchline.
- **Use parenthetical asides.** They're good for an honest reaction, a quick tangent, or deflating your own seriousness (like this). Models rarely interrupt themselves; people do.
- **A plain hedge is human; a stacked hedge is slop.** "I think," "probably," "kind of" are fine and honest. "Could potentially possibly" is not. One qualifier, max.
- **Numbers as digits.** "3 million," not "three million," in most prose.
- **Don't pad to seem thorough.** Shorter and accurate beats longer and fluffy. Never add a sentence whose only job is to look complete.
- **Do the thing instead of announcing it.** No "Let's dive in," "Here's what you need to know," "In this section we'll explore." Just start.
- **End when you're done.** No "In conclusion, the future looks bright." Stop at the last real point, or end on a concrete next step.
- **Cut the hedge stack and the filler.** "may affect," not "could potentially possibly affect." "To do X," not "in order to do X."
- **No decorative formatting.** No emojis in headings, no mechanical boldface, no title-case headings, sentence case instead.

---

## Patterns to avoid (with the human alternative)

### Content

**1. Significance / legacy inflation.** Don't puff up how an arbitrary thing represents a broader trend.
Watch: *stands/serves as, a testament/reminder, pivotal/crucial moment, underscores its importance, reflects broader, marking a shift, evolving landscape, indelible mark, deeply rooted.*
- Slop: `Established in 1989, marking a pivotal moment in the evolution of regional statistics.`
- Human: `Established in 1989 to publish regional statistics independently of Spain's national office.`

**2. Notability padding.** Don't list outlets or follower counts to prove something matters.
- Slop: `Cited in the NYT, BBC, and FT, with an active social media presence of 500k followers.`
- Human: `In a 2024 NYT interview, she argued AI regulation should target outcomes, not methods.`

**3. Superficial -ing tails.** Don't bolt present participles onto sentences for fake depth.
Watch: *highlighting…, ensuring…, reflecting…, showcasing…, fostering…, contributing to….*
- Slop: `The palette resonates with the region, symbolizing local bluebonnets and reflecting a deep connection to the land.`
- Human: `The architect chose blue, green, and gold to reference local bluebonnets and the Gulf coast.`

**4. Promotional / brochure tone.** Don't sell. Describe.
Watch: *boasts, vibrant, rich, nestled, in the heart of, breathtaking, must-visit, renowned, stunning, groundbreaking.*
- Slop: `Nestled in the breathtaking Gonder region, the town stands as a vibrant hub of rich cultural heritage.`
- Human: `A town in Ethiopia's Gonder region, known for its weekly market and 18th-century church.`

**5. Vague attribution.** Don't attribute to phantom authorities. Name the source or drop the claim.
Watch: *experts argue, observers have noted, industry reports, some critics say.*
- Slop: `Experts believe it plays a crucial role in the regional ecosystem.`
- Human: `It supports several endemic fish species, per a 2019 Chinese Academy of Sciences survey.`

**6. Formulaic "Challenges and Future Prospects" sections.** Don't bolt on a generic challenges/outlook section. Write the specific facts.
- Slop: `Despite its prosperity, the city faces challenges typical of urban areas. Despite these, it continues to thrive.`
- Human: `Traffic worsened after three IT parks opened in 2015. A stormwater project began in 2022 to address flooding.`

### Language and grammar

**7. Overused AI vocabulary.** These appear far more in post-2023 text and cluster together. Reach for plainer words.
Watch: *delve, crucial, pivotal, landscape, tapestry, testament, underscore, intricate, interplay, garner, foster, enhance, vibrant, showcase, align with, additionally.*
- Slop: `An enduring testament to Italian influence is the adoption of pasta in the local culinary landscape, showcasing its integration.`
- Human: `Pasta, introduced during Italian colonization, is still common, especially in the south.`

**8. Copula avoidance.** Use is/are/has. Don't dress them up.
Watch: *serves as, stands as, represents, boasts, features, offers.*
- Slop: `Gallery 825 serves as the exhibition space and boasts over 3,000 sq ft.`
- Human: `Gallery 825 is the exhibition space and has about 3,000 sq ft.`

**9. The negate-then-correct construction (FATAL).** This is the single most damning AI tell, so treat it as a hard fail. Any sentence that knocks down one framing and asserts a "corrected" one in its place. All of these are banned:
- `This isn't X. This is Y.`
- `Not X. Y.`
- `Forget X. This is Y.`
- `Less X, more Y.`
- `It's not just X, it's Y.` / `It's not merely a song, it's a statement.`
- `Not only… but…`
- The cleft form: `What made it work wasn't X. It was Y.` / `What got me wasn't X, it was Y.` (see also §34)
- Tailing negations bolted onto the end: `…, no guessing.` / `…, no wasted motion.`

If even one of these appears, the draft has failed. **Delete the negation and just state the positive claim.**
- Slop: `It's not just a song, it's a statement.` / `This isn't a tool. This is a revolution.`
- Human: `The song is a statement.` / `The tool changes how teams ship code.`
- Slop: `The options come from the item, no guessing.`
- Human: `The options come from the selected item, so the user never has to guess.`

**10. Rule of three.** Don't force ideas into triplets to sound complete.
- Slop: `Expect innovation, inspiration, and industry insights.`
- Human: `Expect talks and panels, with time to talk between sessions.`

**11. Synonym cycling (elegant variation).** Don't rotate synonyms for the same thing across sentences. Repeat the plain noun.
- Slop: `The protagonist faces challenges. The main character overcomes them. The hero returns home.`
- Human: `The protagonist faces many challenges but eventually triumphs and returns home.`

**12. False ranges.** Don't write "from X to Y" when X and Y aren't on a real scale.
- Slop: `From the Big Bang to the cosmic web, from the birth of stars to the dance of dark matter.`
- Human: `The book covers the Big Bang, star formation, and current dark-matter theories.`

**13. Passive voice / dropped subjects.** Name the actor when active voice is clearer.
- Slop: `No configuration file needed. Results are preserved automatically.`
- Human: `You don't need a config file. The system saves your results automatically.`

### Style

**14. Em dashes and en dashes — cut them entirely.** This is a hard constraint, not a preference. The em dash is the single most reliable AI tell. Replace each one with a period, comma, colon, parentheses, or a restructure. Catch spaced em dashes ( — ) and double hyphens ( -- ) too.
- Slop: `The policy — announced without warning — affects thousands.`
- Human: `The policy, announced without warning, affects thousands.`
Before shipping, scan the text for `—` and `–`. Any hit means it's not done.

**15. Mechanical boldface.** Don't bold phrases reflexively. Bold sparingly, if at all.

**16. Inline-header bullet lists.** Don't write `- **Thing:** sentence restating the thing.` Write a real sentence or a clean list.
- Slop: `- **Performance:** Performance was enhanced via optimized algorithms.`
- Human: `Load times dropped after the queries were optimized.`

**17. Title-case headings.** Use sentence case. `## Strategic negotiations`, not `## Strategic Negotiations And Partnerships`.

**18. Emojis as decoration.** No 🚀💡✅ on headings or bullets in serious writing.

**19. Curly quotes.** Use straight quotes (`"`) in plain-text contexts like code, commits, and markdown source. (Curly quotes alone are weak evidence; editors auto-curl. Don't obsess, but prefer straight in technical text.)

### Communication artifacts

**20. Chatbot framing.** Never leave assistant chatter in delivered content: "Great question!", "Here's an overview…", "I hope this helps!", "Want me to expand?". Just deliver the content.

**21. Cutoff disclaimers and speculative gap-filling.** Don't write *about* not finding a source, then invent filler. State what's unknown, or cut the sentence.
Watch: *as of my last update, while details are limited, it is believed that, likely grew up, maintains a low profile, keeps personal details private.*
- Slop: `Details of her early life are not publicly available, suggesting she keeps a low profile. She likely grew up middle-class.`
- Human: `Her early life isn't documented in the available sources.` (or omit)

**22. Sycophancy.** Drop "You're absolutely right!", "Excellent point!", "Great question!".

### Filler and hedging

**23. Filler phrases.** "in order to" → "to"; "due to the fact that" → "because"; "at this point in time" → "now"; "has the ability to" → "can"; "it is important to note that" → (just say it).

**24. Hedge stacks.** "could potentially possibly" → "may". One qualifier max.

**25. Generic upbeat conclusions.** Replace "the future looks bright, exciting times ahead" with a concrete fact or next step.

**26. Hyphenated-pair overuse.** Keep the hyphen when the compound is attributive (`a high-quality report`); drop it after the noun (`the report is high quality`). AI hyphenates uniformly; humans don't.

**27. Persuasive-authority tropes.** Don't pretend to cut to a deeper truth: "the real question is," "at its core," "what really matters," "fundamentally." Usually it just restates an ordinary point with ceremony.

**28. Signposting.** Don't announce; do. Cut "let's dive in," "let's explore," "here's what you need to know," "now let's look at."

**29. Fragmented headers.** Don't follow a heading with a one-line restatement before the real content. Start with the content.

**30. Diff-anchored writing.** Unless it's a changelog or migration guide, describe the thing as it is, not as a change from before. `This uses a hash map for O(1) lookups`, not `This was added to replace the old O(n²) loop`.

**31. Manufactured punchlines / staccato drama.** Don't stack short fragments to fake intensity. One short sentence for emphasis is fine; a run of them sounds engineered.
- Slop: `It had no preference for symmetry. No aesthetic prior. No nostalgia. The old rules were gone.`
- Human: `It didn't favor symmetry or human-looking designs, which made some older assumptions less useful.`

**32. Aphorism formulas.** Avoid "X is the language of Y," "X becomes a trap," "the architecture of Z." Say the concrete claim instead.
- Slop: `Symmetry is the language of trust.`
- Human: `Symmetric layouts tend to feel more predictable to users.`

**33. Fake-candid openers.** Drop standalone "Honestly?", "Look,", "Here's the thing," "Real talk" used as a theatrical pause before an ordinary point. A person being honest just says the thing.

**34. Cleft-sentence reveals and agency-swap punchlines.** The wh-cleft ("What got me is…", "What struck me was…", "What made it work wasn't X. It was Y.") stages an ordinary observation as a revelation, and it usually lands on a too-clever inversion where the abstract thing acts on the writer ("The anxiety recalibrated before I did," "the tool was training me"). The negated cleft is §9 wearing a costume; the inversion is a slogan posing as introspection. State the observation directly and keep the agency where it belongs.
- Slop: `What got me is that I didn't reason my way there. The anxiety recalibrated before I did.`
- Human: `I noticed the anxiety had faded before I had any argument for why it should.`
- Slop: `What made the demo land wasn't the model. It was the silence in the room.`
- Human: `The room went quiet during the demo. That told me more than the benchmarks did.`

### Social media

Feed posts (X, LinkedIn, Mastodon, Threads) follow every rule above, plus three of their own.

**35. The buried lede.** The first line decides whether anyone reads the rest. LinkedIn truncates after roughly two lines; on X the opener is the whole impression. Lead with the most specific, surprising fact you have. Cut the setup and the throat-clearing.
- Slop: `I've been thinking a lot about developer productivity lately, and I wanted to share a few observations from our team's journey.`
- Human: `We deleted 40% of our CI config last month. Builds got 6 minutes faster.`

**36. Broetry.** Short paragraphs with whitespace are native feed formatting; use them so the post survives a phone screen. Broetry is the slop version: every line its own dramatic paragraph, each a fake revelation. §31 applies here with full force. The test is the same: does each line carry content, or just rhythm?
- Slop: `I failed.` / `Publicly.` / `And it was the best thing that ever happened to me.` (each on its own line)
- Human: `My first launch flopped: 12 signups, 9 of them friends. The postmortem taught me more than the build did.`

**37. Engagement-bait CTAs and the announcement template.** Generic closers ("Thoughts?", "Agree?", "Repost if this resonated") are bait; a specific question to a specific audience is human. The announcement-post template is as recognizable as an em dash now: "I'm humbled/thrilled to announce," hook + numbered list + "follow me for more," "Let's connect!", the 🧵 emoji.
- Slop: `🚀 Thrilled to announce I'm joining Acme as VP of Engineering! Huge thanks to everyone who believed in me. Let's connect!`
- Human: `New job: VP of Engineering at Acme. First project is fixing the deploy pipeline I complained about here in March.`
- Slop: `Thoughts? ♻️ Repost if this resonated.`
- Human: `If you've shipped this on Postgres 16, I want to hear how the migration went.`

---

## Personality and soul

Avoiding tells is only half the job. Sterile, voiceless prose is as obviously machine-made as slop. **Apply this only where the register allows it** (essays, opinion, blog posts, personal writing). For reference, technical, legal, and most docs, neutral and plain *is* the right human voice. Don't inject opinions or first person there.

Signs your "clean" writing is soulless: every sentence the same length, pure neutral reporting, no opinion, no acknowledged uncertainty, no first person where it fits, reads like a press release.

How to add a pulse, when appropriate:
- **Have a take.** React to facts, don't just list them. "I genuinely don't know how to feel about this" is more human than balanced pros and cons.
- **Vary rhythm deliberately.** Short and punchy, then long and winding.
- **Let some mess in.** A tangent, an aside, a half-formed thought, a self-correction.

Soulless: `The experiment produced interesting results. 3M lines of code were generated. Some were impressed, others skeptical. The implications remain unclear.`
Has a pulse: `I don't know how to feel about this one. 3 million lines of code, generated while we slept. Half the dev world is losing it, half are explaining why it doesn't count. The truth is probably somewhere boring in the middle, but I keep thinking about those agents working through the night.`

---

## Voice matching (when a sample exists)

If the user gives a writing sample or points to existing house style, read it before drafting and copy its mechanics: sentence-length pattern, formality level, how paragraphs open, punctuation habits, recurring phrases, how transitions are handled. Don't just remove AI patterns; replace them with patterns from the sample. If they write "stuff" and "things," don't upgrade to "elements" and "components." A real sample overrides every default in this skill.

---

## What NOT to over-correct (false positives)

Don't gut legitimate prose chasing tells. On their own, these are **not** evidence of AI:
- Polish and consistent style (the writer may be a pro or edited).
- Formal or academic vocabulary (AI overuses *specific* words, §7, not all big words). Keep "ostensibly," "constituent."
- One em dash, one curly quote, or one "however" in isolation. Tells matter in **clusters**.
- One short emphatic sentence. Flag staccato only when several pile up.
- Dry or "robotic" prose without the specific tells. Dry is just dry.
- Unsourced claims (most writing is unsourced).

When unsure, look for a cluster: a single em dash means nothing; em dashes + rule-of-three + "vibrant tapestry" + a "Conclusion" section is a confession.

**Preserve these human signals** if they're already in the text: hard-to-fabricate specific detail, mixed feelings and unresolved tension, dated/era-bound references, defensible first-person choices, varied sentence length, genuine asides and self-corrections.

---

## Banned phrases (when you're the one writing)

The false-positive guidance above is for *editing someone else's* text, where you weigh clusters and context. When **you** are the one generating, there's no judgment call: just never emit the phrases below. They're nearly always slop.

**Dead AI language:** in today's [anything], it's important/worth noting that, delve, dive into, unpack, harness, leverage, utilize, landscape, realm, robust, game-changer, cutting-edge, straightforward, I'd be happy to help, in order to.

**Dead transitions:** furthermore, additionally, moreover, moving forward, at the end of the day, to put this in perspective, what makes this particularly interesting is, the implications here are, in other words, it goes without saying.

**Engagement bait:** let that sink in, read that again, full stop, this changes everything, are you paying attention, you're not ready for this, thoughts?, agree?, repost if this resonated, drop a comment below.

**Announcement-post tells:** humbled to announce, thrilled to announce/share, excited to share some news, beyond grateful, let's connect, follow me for more, the 🧵 emoji.

**Hype / AI cringe:** supercharge, unlock, future-proof, 10x your productivity, the AI revolution, in the age of AI.

**Fake-insider claims:** here's the part nobody's talking about, what nobody tells you, most people don't realize, anything built on "nobody."

**Manufactured insight (see §34):** what got me is, what struck me was, what surprised me wasn't, and any punchline where the abstraction acts on the writer ("the anxiety recalibrated before I did").

**Fatal (see §9):** any negate-then-correct sentence. "This isn't X, it's Y." "Not X. Y." "Less X, more Y." "Forget X." "What made it work wasn't X. It was Y." Delete the negation; state the positive.

(Register caveat: a word like "robust" or "leverage" can be legitimate in a specific technical sense, e.g. "robust to outliers." The ban is on the empty rhetorical use, not the precise one.)

---

## Self-audit (run before shipping)

1. **Em/en dash scan.** Search for `—` and `–`. Zero allowed. Also check ` -- ` and spaced ` - ` used as a dash.
1a. **Fatal negation scan (§9).** Search for any "this isn't X, it's Y," "not X, Y," "less X more Y," "not just… but…" sentence. One is a failure. Delete it and state the positive claim.
1b. **Banned-phrase scan.** Skim the banned list above. If you wrote one, replace it.
2. **Read it aloud in your head.** Does the rhythm vary, or is every sentence the same mid-length beat? Find the longest sentence and ask whether it should be two or three.
2a. **Transition check.** Could you delete "additionally / moreover / furthermore / as such" and just let the sentences sit next to each other? Usually yes.
3. **Ask: "What here would make a reader think a model wrote it?"** Name the remaining tells honestly (a clean contrast, a tidy triplet, a slogan-y closer) and fix them.
4. **Check the open and close.** No signposting at the start, no generic uplift at the end.
5. **Specificity check.** Did you state facts, names, numbers, and dates, or did you gesture at significance? Prefer the concrete.
6. **Register check.** Does the voice match the medium? Personality only where it belongs.
7. **Feed-post check.** If it's a social post: the most specific fact is in line 1, the paragraphs survive a phone screen, and the closer is a real question or nothing (§35–37).

If you can search the draft with a tool, grep for the highest-signal tells:

```
grep -niE "—|–|this is ?n.t [^.]+\.? *(this is|it.s)|not just[^,]*,? *(it.s|but)|less [^,]+, more|serves as|stands as|testament|pivotal|delve|dive into|leverage|utilize|robust|landscape|in order to|furthermore|additionally|moreover|let.s (dive|explore)|let that sink in|game.?changer|supercharge|10x|nobody.s talking|I hope this helps|the future looks bright|humbled to|thrilled to (announce|share)|let.s connect|follow me for|repost if|what (got|struck|surprised) me|wasn.t [^.]+\. it was" draft.md
```

---

## Reference and attribution

Based on [Wikipedia:Signs of AI writing](https://en.wikipedia.org/wiki/Wikipedia:Signs_of_AI_writing) (WikiProject AI Cleanup, CC BY-SA 4.0) and the [humanizer skill](https://github.com/blader/humanizer) by Siqi Chen (MIT). Reframed here as proactive guidance for agents writing prose, rather than a cleanup pass. License and attribution details: see NOTICE.md in this repository.

Key idea from Wikipedia: "LLMs use statistical algorithms to guess what should come next. The result tends toward the most statistically likely result that applies to the widest variety of cases." Good writing is the opposite of the most likely next token.
