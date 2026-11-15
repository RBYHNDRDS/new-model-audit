# New Model Audit

A portable AI skill that turns every new model release into an audit of your own setup.

Most people test a new model with a few random prompts. That tells you nothing about how it handles your actual work. This skill hands the model your real files (brand docs, offer docs, claims list, briefs, prompts, skills, angle logs) and has it report what contradicts, what is out of date, what is missing, and which rules only exist because an older model needed them. Then it remakes one job you already finished so you can compare old and new without knowing which is which.

It is written for DTC and ecom teams. The method works for any team that keeps its instructions in files.

## What it does

- Lists every file it read, so you can see what the audit is based on.
- Finds contradictions between files: offers, claims, customer, voice, product names.
- Flags what looks outdated, and keeps a separate "ask the team" list for what it cannot confirm.
- Lists what is missing, ranked by how much it would improve the work.
- Reviews your recent briefs and names the fields your template lacks.
- Walks through your ad workflow and lists the rules worth testing without.
- Proposes ten changes, ranked, and the three to do today.
- Remakes one finished job and shows old and new as A and B.

Every finding comes with the file name and the quoted line. Nothing in your setup is edited until you pick a change.

## Included files

- `SKILL.md`: the complete agent workflow.
- `agents/openai.yaml`: optional UI metadata for OpenAI-compatible skill hosts.

## Requirements

An agent that can read a folder of files. No scripts, no packages, no API keys.

## Install

Clone the repository:

```bash
git clone https://github.com/RBYHNDRDS/new-model-audit.git
```

For Codex and other agents that scan `~/.agents/skills`:

```bash
mkdir -p "${HOME}/.agents/skills"
ln -s "${PWD}/new-model-audit" "${HOME}/.agents/skills/new-model-audit"
```

For Claude Code:

```bash
mkdir -p "${HOME}/.claude/skills"
ln -s "${PWD}/new-model-audit" "${HOME}/.claude/skills/new-model-audit"
```

## Use it

Ask in normal language:

```text
Use $new-model-audit on my brand folder.
The setup lives in ./brand. For the retest, use briefs/spring-launch.md
and the script we shipped from it.
```

Before you start:

- Put everything in one place, including a few ads that worked and a few that did not, with the numbers.
- Leave out anything you are not allowed to share with an AI tool, such as customer data or contracts.
- Make a backup copy of the folder.
- Pick one finished job you were happy with. The retest needs it.

## Privacy and safety

- The audit is read-only. Changes happen one at a time and only after you choose them.
- Files stay local. The skill tells the agent not to send them to any outside service.
- If the agent finds a password, key or customer record, it reports where it is and does not repeat the value.
- No scripts, telemetry or credential readers are included.

## License

MIT. See `LICENSE`.
