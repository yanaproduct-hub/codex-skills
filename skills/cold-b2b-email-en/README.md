# cold-b2b-email-en

Codex skill for English-language B2B cold emails and follow-up sequences.

The skill helps write first-touch emails and 3-5 step follow-up sequences that sound like a strong B2B seller: specific, concise, human, and low-pressure.

## Use It For

- first-touch B2B cold email
- 3-5 step outbound sequence
- getting a reply
- booking a call
- getting routed to the right decision-maker
- asking permission to send a pilot plan
- inviting a prospect to a demo
- reviving a silent thread

## How It Works

On launch, the skill asks:

1. What is the goal of the email?
2. What result should this email create?

Then it clarifies:

- target role, company type, segment, and seniority
- whether you need one email or a 3-5 step sequence
- whether versions are needed by pain, role, segment, industry, or trigger
- whether to include a link and why
- which proof points are allowed
- banned words, claims, or compliance limits
- the next sales step

If project context exists, the skill uses it: `AGENTS.md`, `.agents/product-marketing-context.md`, `.claude/product-marketing-context.md`, sales notes, or call transcripts.

## Install

From the cloned repository root:

```bash
mkdir -p ~/.codex/skills
cp -R skills/cold-b2b-email-en ~/.codex/skills/
```

Or in one flow:

```bash
git clone https://github.com/yanaproduct-hub/codex-skills.git
mkdir -p ~/.codex/skills
cp -R codex-skills/skills/cold-b2b-email-en ~/.codex/skills/
```

## Example Prompt

```text
Use cold-b2b-email-en. Write a first-touch email and a 4-step follow-up sequence for VP People buyers. Goal: get permission to send a pilot plan.
```

## What's Inside

```text
cold-b2b-email-en/
  README.md
  SKILL.md
  agents/
    openai.yaml
  references/
    outbound-mechanics.md
    project-adaptation.md
    quality-checklist.md
```

## Native English Notes

- Keep subject lines short and plain.
- Lead with the prospect's world, not your company intro.
- Use understated confidence, not hype.
- Avoid translated-formal phrasing and long sender introductions.
- Avoid "I hope this email finds you well", "I came across your profile", "synergy", "leverage", and "best-in-class".
- Use one low-friction CTA that can be answered in one line.

## References

- [`outbound-mechanics.md`](references/outbound-mechanics.md): first email mechanics, CTAs, subjects, follow-ups, and links.
- [`project-adaptation.md`](references/project-adaptation.md): project adaptation, buyer lenses, proof points, and banned claims.
- [`quality-checklist.md`](references/quality-checklist.md): final quality review for emails and sequences.

## Safety

The skill is text-only. It contains no scripts, tokens, network calls, or hidden automation.

For sensitive categories, it asks for project-specific restrictions before writing: medical claims, financial promises, internal metrics, customer names, legal limits, or banned product terms.

For scaled outbound, users are responsible for legal compliance, sender reputation, bounce rate, spam complaints, unsubscribe handling, and regional rules.

## Release

- [`v0.2.1`](https://github.com/yanaproduct-hub/codex-skills/releases/tag/v0.2.1)
