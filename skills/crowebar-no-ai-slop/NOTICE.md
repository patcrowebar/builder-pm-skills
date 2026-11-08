# Notice

crowebar-no-ai-slop is maintained by Pat Crowe (Crowebar Labs). It is an independent version, not the original no-ai-slop, and is not maintained or endorsed by Peter Yang or Ruben Hassid. It builds on two MIT-licensed projects. The MIT License requires keeping each original copyright and permission notice with copies of the software, so both are kept below.

## 1. no-ai-slop by Peter Yang

Source: https://github.com/petergyang/no-ai-slop
License: MIT, Copyright (c) 2026 Peter Yang

crowebar-no-ai-slop started from Peter Yang's no-ai-slop. `SKILL.md` and `eval.md` keep its approach and much of its content: the editor stance, the editing principles, the words and patterns to cut, and the pass/fail eval.

Changes since then include voice preservation and minimum-effective-edit rules, a Detect mode, the X posts and replies section, and the Humanizer material listed in section 2.

### License text

MIT License

Copyright (c) 2026 Peter Yang

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
SOFTWARE.

## 2. Humanizer by Ruben Hassid (How to AI)

Source: Humanizer skill, version 2.0.0
License: MIT

`scripts/tells.py`, `assets/tells.json`, and `assets/examples.json` are adapted from Humanizer. Ideas folded into `SKILL.md` and `eval.md` include the fact guard, register guidance ("humanizing is not casualizing"), boilerplate by kind of writing, literal-use exceptions, and the rhythm checks.

Changes for crowebar-no-ai-slop (November 2026):

- Added lexicon entries for the skill's rhetorical patterns: binary contrasts, colon reveals, faux-insight setups, interpretive metadiscourse, rhetorical setups, negative listing, dramatic fragmentation, weasel attribution, and others (entries tagged `"src": "crowebar-no-ai-slop"`).
- Added a test/eval harness exception to "harness."
- Added two verified X examples (post and reply).
- Renamed the script's output headers and added the `x` register.

### License text

Humanizer did not ship with a LICENSE file. Its SKILL.md declares `license: MIT` and credits "How to AI by Ruben Hassid," so the standard MIT text is used below. The copyright line is taken from that metadata and has not been confirmed with Ruben Hassid (as of 8 November 2026). If you are Ruben and want it worded differently, open an issue on this repository and it will be corrected.

MIT License

Copyright (c) 2026 Ruben Hassid (How to AI)

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
SOFTWARE.
