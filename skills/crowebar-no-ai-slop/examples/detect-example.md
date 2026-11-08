# Detect example: a customer email

## Prompt

> Does this read like AI slop? Don't rewrite it, just flag what's wrong.
>
> Subject: Exciting Changes to Your Plan!
>
> Hi Jordan,
>
> I hope this email finds you well. We're thrilled to announce that starting March 1, your Starter plan will include unlimited projects — a game-changer for teams like yours. This isn't just an upgrade. It's a whole new way to work.
>
> Whether you're a solo founder or a growing team, our robust platform empowers you to do more. Please don't hesitate to reach out with any questions!
>
> Best,
> Sam

## Response

```
Patterns found

Email boilerplate
- "I hope this email finds you well" → cut it; open with the news.
- "Please don't hesitate to reach out with any questions!" → cut it, or say "Reply to this
  email with questions."

Announcement template
- "We're thrilled to announce" → announce it plainly: "Starting March 1, your Starter plan
  includes unlimited projects."
- "Exciting Changes to Your Plan!" (subject) → name the change: "Unlimited projects on Starter
  from March 1."

Binary contrast
- "This isn't just an upgrade. It's a whole new way to work." → say what it is, or cut it.

Audience catch-all
- "Whether you're a solo founder or a growing team" → you're writing to Jordan; drop it.

Banned words
- "game-changer," "robust," "empowers" → cut, and say what actually changes for Jordan.

Punctuation
- One em dash ("projects — a game-changer") → use a period.
- Two exclamation marks → keep one at most.

The only real news is one fact: unlimited projects on Starter from March 1. Want me to edit
it down?
```

## Why this is a good response

- Names each pattern and quotes the exact line, so the writer can check every finding.
- Doesn't rewrite the email, show a score, or guess whether AI wrote it.
- Catches the subject line, which the scanner doesn't flag; the skill's own judgment does.
- Ends by offering the edit instead of doing it uninvited.
