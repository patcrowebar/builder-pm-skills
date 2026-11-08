# Changelog

## 1.0.0 (2026-11-08)

First public release of the Crowebar version.

- Built on Peter Yang's no-ai-slop: editor stance, editing principles, words and patterns to cut, and a pass/fail eval
- Voice preservation and minimum-effective-edit rules
- Detect mode: names patterns with quoted lines, without rewriting or scoring
- X posts and replies section, based on X's open-source ranking code
- Folded in material adapted from Ruben Hassid's Humanizer:
  - Bundled scanner (`scripts/tells.py`) with a lexicon of about 250 entries, each with a reason and a fix
  - Fact guard: checks that numbers, dates, times, links, emails, and handles survive an edit, and flags anything invented
  - Register guidance: humanizing is not casualizing; formal writing stays formal
  - Boilerplate by kind of writing: chatbot leakage, email, support replies, condolences, bios, cover letters, announcements
  - Literal-use exceptions (robust in statistics, foster care, test harness)
  - Rhythm checks: sentence-length variation, same-opener runs, paragraph uniformity
- New lexicon entries so the scanner catches this skill's rhetorical patterns: binary contrasts, colon reveals, faux-insight setups, metadiscourse, rhetorical setups, negative listing
- 12 verified before/after pairs, including an X post and an X reply
- The accent score stays internal and is never shown as an AI-detection verdict
- 8 eval scenarios
