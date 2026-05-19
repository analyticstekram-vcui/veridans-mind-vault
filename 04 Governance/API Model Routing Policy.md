# API Model Routing Policy

This policy controls how Veridan Core and OpenClaw use GPT/API models.

## Core Rule

OpenClaw must use cheaper GPT models by default.

Heavy GPT mode is not allowed unless the operator explicitly approves it.

OpenClaw must stay stopped when not actively being used.

## Operating Modes

### OFF MODE

OpenClaw is stopped.

Use when:
- no active OpenClaw work is needed
- API cost must be zero
- system is idle

Command:

```bash
openclaw-off
