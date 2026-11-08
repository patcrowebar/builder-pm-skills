# Crowebar No AI Slop eval

Use this after the rewrite. Answer each check with pass or fail. If any check fails, fix the draft before returning it.

For detect requests, make sure the response names each pattern found with a quoted line and a short fix, without rewriting the draft.

## Facts

1. Did the fact guard (`compare`) report no errors, and did you check every warning against the original? Without code, did you confirm by hand that every number, name, date, time, and link survived and nothing was added?
2. Did you check names, titles, and company names yourself, since the fact guard can miss them?

## Editing principles

1. Does the edit preserve the user's point without adding claims, examples, stats, quotes, or opinions?
2. Does it preserve the writer's distinctive vocabulary, cadence, bluntness, humor, uncertainty, digressions, and level of polish?
3. Does it leave strong human sentences alone instead of rewriting them for consistency or making every paragraph equally tidy?
4. Is the amount of cutting proportional to the actual slop, with no aggressive compression that strips out character?
5. Does the draft lead with what the reader needs while keeping personal setup that adds context, tension, or character?
6. Are points front-loaded where that improves clarity without forcing every unit into the same structure?
7. Do sentences earn their place, with concrete facts, protected details, and direct verbs where the draft supports them?
8. Does every generic sentence pass the portability test, or was it cut or made specific to this subject?
9. Does the draft use active voice with human subjects where possible?
10. Does the edit keep useful edge and preserve structure unless the structure was hurting the piece?
11. Are genuinely tangled sentences fixed while clear spoken cadence, fragments, and changes in pace remain intact?
12. Were sentences rebuilt around their point rather than fixed by swapping synonyms?
13. If the source was thin, is the edit honestly short, with a request for a real detail instead of invented padding?
14. Do claims have an owner, with at most one hedge where uncertainty is real?

## Register

1. Does the edit match the register? Formal pieces stay formal (no contractions, slang, or casual asides); everyday pieces sound like the writer talking.
2. Is there no faked humanity: no invented typos, injected slang, or forced casualness?

## Words to cut

1. Are banned words, filler phrases, often-empty adverbs, and inflated claims removed unless quoted as examples or used literally?
2. Were banned words replaced with plain words rather than their neighbors (multifaceted, intricate, bolster, garner)?

## Patterns to cut

1. Are binary contrasts, negative listings, rhetorical setups, and throat-clearing openers removed?
2. Are faux-insight setups, colon reveals, superficial analysis, fake-strong verbs, synonym cycling, dramatic fragments, and robotic rhythm fixed?
3. Are importance puffery and weasel attribution replaced with plain facts and named sources, or flagged for the user when no source exists?
4. Are hedge stacks and impersonal instructions ("it is essential to") fixed?
5. Is interpretive metadiscourse removed, including authorial metacommentary, reader guidance, emphasis markers, and redundant glossing?
6. Are audience catch-alls and formula openers ("Whether you're...", "In today's...", "By leveraging...", "Imagine a world...") removed?
7. Is there at most one triple in the piece, unless the content really has three things each time?
8. Are fake-profound kicker lines deleted instead of rewritten into better metaphors?
9. Are summary-recap endings and contentless uplifting sign-offs cut so the piece ends on a concrete point, takeaway, or next action?
10. Is boilerplate for the kind of writing removed: chatbot leakage, email templates, support-desk phrasing, condolence stock lines, bio and cover-letter filler, announcement templates, engagement bait?
11. Is formatting slop removed: Emoji headings or bullets, decorative bold, bold-term bullet lists, bullets that should be prose, headers over tiny sections?
12. Are colons sentence case unless grammar, a proper noun, a title, or code requires otherwise?
13. Are em dashes used sparingly (usually none in short copy, only 1-2 in longer drafts when they clearly help), with no spaced hyphens or "--" swapped in as stand-ins?
14. Are semicolon hinges, suspense ellipses, and extra exclamation marks gone?

## Final read

1. Does the draft avoid robotic symmetry, repeated sentence shapes, same-word sentence openers, and stacked punchy fragments?
2. Would the writer recognize the edited draft as their own voice?
3. Would the edited draft sound natural if read to a sharp colleague?
4. Does the final output include the full edited draft and a short **What changed** section ending with the fact-guard result?
5. Is the accent score kept out of the response, with no claim about AI detectors?
6. For detect requests, does the response name each pattern with a quoted line and a short fix, without rewriting, scoring, or claiming AI authorship?
