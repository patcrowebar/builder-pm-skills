# Builder PM Skills

Agent skills for product managers and AI-native builders, by [Pat Crowe](https://github.com/patcrowebar) / Crowebar Labs.

Each skill is a folder with a `SKILL.md` file that Claude (and other agents that support the SKILL.md format) loads when the task fits. The goal isn't more templates. It's reusable product judgment: the calls an experienced PM makes, packaged so you can run them on demand.

## Skills

| Skill | What it does | Use it when |
|---|---|---|
| [build-to-learn](skills/build-to-learn/) | Decision-first experiment coach. Finds the riskiest belief behind a bet, recommends the one test worth running (or tells you to just decide), and reviews the results honestly afterward. | You're about to build, fund, price, or test something, or you're back with results and need to know what they actually proved. |
| [ux-review](skills/ux-review/) | Reviews or shapes a product experience against a UX thesis of 8 principles and 4 AI-native expectations. Covers full and quick reviews, spec requirements, build-prompt hardening, trade-off calls, AI feature audits, and measurement plans. | You have a screen, flow, spec, build prompt, or AI feature and want specific, testable UX feedback instead of taste. |
| [crowebar-no-ai-slop](skills/crowebar-no-ai-slop/) | Edits drafts into sharper, more human writing while keeping the writer's voice, or flags AI-slop patterns without rewriting. A bundled scanner checks that every number, date, and link survives the edit. Also checks X posts and replies against X's spam and slop rules. | You're about to send or publish something as yourself, or you want to know what makes a draft read like AI. |

More skills are coming.

## Install

### Claude Code

Copy the skill folder into your personal skills directory:

```bash
git clone https://github.com/patcrowebar/builder-pm-skills.git
mkdir -p ~/.claude/skills
cp -r builder-pm-skills/skills/build-to-learn ~/.claude/skills/
cp -r builder-pm-skills/skills/ux-review ~/.claude/skills/
cp -r builder-pm-skills/skills/crowebar-no-ai-slop ~/.claude/skills/
```

To make it available in a single project only, copy it into that project's `.claude/skills/` folder instead.

### Claude apps (claude.ai, desktop, mobile)

1. Download the skill folder (for example, `skills/build-to-learn`).
2. Zip the folder so `SKILL.md` sits at the top level of the zip.
3. Upload the zip in Claude's skills settings.

### skills CLI

```bash
npx skills add https://github.com/patcrowebar/builder-pm-skills --skill build-to-learn
```

## Using a skill

Skills load automatically when your request matches their description. You can also call one directly by name, for example `/build-to-learn`.

Each skill folder includes:
- `SKILL.md`: the instructions the agent follows
- `README.md`: the human guide, covering when to use it and what to expect
- `examples/`: sample runs
- `evals/`: test prompts with expected behavior, for checking that the skill still works after you change it
- `CHANGELOG.md`: version history

## Repo structure

```
builder-pm-skills/
├── README.md
├── LICENSE
└── skills/
    ├── build-to-learn/
    │   ├── SKILL.md
    │   ├── README.md
    │   ├── CHANGELOG.md
    │   ├── examples/
    │   │   ├── plan-example.md
    │   │   └── review-example.md
    │   └── evals/
    │       └── evals.json
    ├── ux-review/
    │   ├── SKILL.md
    │   ├── README.md
    │   ├── CHANGELOG.md
    │   ├── examples/
    │   │   ├── quick-review-example.md
    │   │   └── tradeoff-example.md
    │   └── evals/
    │       └── evals.json
    └── crowebar-no-ai-slop/
        ├── SKILL.md
        ├── README.md
        ├── CHANGELOG.md
        ├── NOTICE.md
        ├── eval.md
        ├── scripts/
        │   └── tells.py
        ├── assets/
        │   ├── tells.json
        │   └── examples.json
        ├── examples/
        │   ├── edit-example.md
        │   └── detect-example.md
        └── evals/
            └── evals.json
```

## Feedback

Found a case where a skill gave bad advice? Open an issue with the prompt you used and what you expected. Those cases become new evals.

Pull requests aren't being accepted right now. Issues and suggestions are welcome.

## License

[MIT](LICENSE). `crowebar-no-ai-slop` also includes MIT-licensed material from Peter Yang's [no-ai-slop](https://github.com/petergyang/no-ai-slop) and Ruben Hassid's Humanizer; see its [NOTICE.md](skills/crowebar-no-ai-slop/NOTICE.md).
