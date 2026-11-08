# crowebar-no-ai-slop

**Edit drafts into sharper, more human writing without losing the writer's voice or facts.**

Most "humanizer" tools swap words and call it done. The robotic skeleton stays: "It's not just X, it's Y," the colon reveal, the closing line that tries to sound deep. This skill rebuilds sentences around their point, keeps what makes the writer sound like themselves, and then checks its own work. A bundled scanner confirms that every number, date, and link in the original survived the edit and that nothing was invented.

This is Crowebar Labs' independent version. It builds on [Peter Yang's no-ai-slop](https://github.com/petergyang/no-ai-slop) and Ruben Hassid's Humanizer. It isn't the original version of either, and neither author maintains or endorses it. See [Credits](#credits).

## Modes

| Mode | Use it for | You get |
|---|---|---|
| **Edit** (default) | Any draft you'll send or publish as yourself | The full edited draft and a short What changed section, ending with whether every fact was kept |
| **Detect** | "Is this AI slop?" or an audit without a rewrite | Each pattern named, with the quoted line and a short fix. No rewrite, no score, no guess about whether AI wrote it |

X posts and replies also get a separate check against X's spam and slop rules, based on X's open-source code.

## What it catches

- **Rhetorical patterns:** binary contrasts, faux-insight setups ("the part everyone misses"), colon reveals, metadiscourse ("that last part matters"), fake-profound kickers, summary-recap endings
- **Stock words and phrases:** delve, leverage, seamless, game-changer, "in today's fast-paced world," and more, about 250 entries in all, with exceptions for literal uses
- **Boilerplate by kind of writing:** chatbot leakage, email templates, support replies, condolences, bios, cover letters, announcements
- **Rhythm and formatting:** sentences that all run the same length, runs of identical openers, triples in every paragraph, decorative bold and emoji, em dashes used as a crutch

## What makes it different

- **It keeps the writer.** Strong human sentences stay. Fragments, bluntness, and "honestly" stay when they belong to the writer.
- **It never invents.** No new facts, stats, examples, or quotes. If the draft is thin, the edit stays short and the skill asks for one real detail.
- **It checks facts mechanically.** The fact guard compares before and after and flags anything lost or added.
- **Formal stays formal.** A condolence note or board memo loses its template phrases, not its register.
- **No detector theater.** The internal score counts style patterns. It isn't an AI detector, and the skill never promises a text will pass one.

## Examples

- [Edit](examples/edit-example.md): a building-in-public post
- [Detect](examples/detect-example.md): a customer email

Twelve more verified before/after pairs (emails, posts, X, bio, cover letter, blurb, intro, announcement, condolence, board memo) are in [`assets/examples.json`](assets/examples.json). Run `python3 scripts/tells.py example` to list them.

## Requirements

The scanner needs Python 3 with no extra packages. Without code execution, the skill does the same checks by hand.

## Testing changes

[`evals/evals.json`](evals/evals.json) holds test prompts covering both modes, voice preservation, invented facts, formal register, X replies, literal uses, and the em-dash rule. [`eval.md`](eval.md) is the checklist the skill runs on its own output. After changing [`assets/tells.json`](assets/tells.json), run `python3 scripts/tells.py example` and confirm every pair still passes.

## Credits

Built on two MIT-licensed projects:

- [no-ai-slop](https://github.com/petergyang/no-ai-slop) by Peter Yang, the starting point for the instructions and eval
- Humanizer by Ruben Hassid (How to AI), the source of the scanner, lexicon, and examples

Full license notices are in [`NOTICE.md`](NOTICE.md).
