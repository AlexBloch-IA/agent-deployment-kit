# Agent Deployment Kit

> Replicate one agent across N clients without drift — one context source, a generator that refuses unknowns. Use when duplicating an agent deployment. Trigger on "duplicate this agent", "same bot new client", "the agent named the wrong client".

[![License: MIT-0](https://img.shields.io/badge/License-MIT--0-blue.svg)](https://opensource.org/licenses/MIT-0)
[![ClawHub](https://img.shields.io/badge/ClawHub-Published-orange)](https://clawhub.ai/alexbloch-ia/skills/agent-deployment-kit)
[![Version](https://img.shields.io/badge/version-1.1.0-green)](https://clawhub.ai/alexbloch-ia/skills/agent-deployment-kit)

A Claude Code / [OpenClaw](https://openclaw.ai) skill, published on [ClawHub](https://clawhub.ai/alexbloch-ia/skills/agent-deployment-kit). Portable operating doctrine — drop it into an agent's skills directory and follow it.

---

## What the doctrine covers

- Kit anatomy
- The context contract
- The generator you write
- Rule 1
- Absolute rules
- Absolute rules (HARD-CODED
- Rule 2
- Rule 3
- Field of vision: why AGENTS.md duplicates the guardrails
- Pre-deploy audit (go/no-go)
- Recontextualising an existing kit
- Gotchas

The full, load-bearing detail lives in [`SKILL.md`](./SKILL.md).

---

## Install

### Via ClawHub (recommended)

👉 **<https://clawhub.ai/alexbloch-ia/skills/agent-deployment-kit>**

```bash
clawhub install agent-deployment-kit
# or, from an OpenClaw agent:
openclaw skills install @alexbloch-ia/agent-deployment-kit
```

### Via this repository (manual)

```bash
git clone https://github.com/AlexBloch-IA/agent-deployment-kit.git
cd agent-deployment-kit
./install.sh
```

The script copies the full skill payload into every supported stack it finds:

- `~/.claude/skills/agent-deployment-kit/` (Claude Code)
- `~/.openclaw/skills/agent-deployment-kit/` (OpenClaw)

### Manual copy

```bash
mkdir -p ~/.claude/skills/agent-deployment-kit
cp -R SKILL.md ~/.claude/skills/agent-deployment-kit/   # plus scripts/, references/, templates/… if present
```

---

## Repository structure

```
agent-deployment-kit/
├── SKILL.md
├── context/
├── README.md
├── LICENSE
└── install.sh
```

---

## License

Released under **MIT-0** (MIT No Attribution). Use, fork, adapt, redistribute — no attribution required.

---

## Author

[Alexandre Bloch](https://github.com/AlexBloch-IA) — founder of [OpenClaw](https://openclaw.ai).
Published on [ClawHub](https://clawhub.ai/alexbloch-ia).
