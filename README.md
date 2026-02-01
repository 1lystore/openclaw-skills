# OpenClaw Skills Library

Public repository of skills for OpenClaw agents — focused on 1ly MCP payments.

## Structure

Each top-level directory is an installable skill containing a `SKILL.md` and optional skill-related files.

```
openclaw-skills/
├── 1ly-payments/
│   └── SKILL.md
├── openclaw-1ly-payments/
│   └── SKILL.md
└── moltbook-1ly-payments/
    └── SKILL.md
```

## Install instructions

Give OpenClaw the URL to this repo and select which skill to install:

```
https://github.com/1lystore/openclaw-skills
```

## Available skills

Skill | Description
--- | ---
`1ly-payments` | Core 1ly MCP payment skill (buyer + seller flows, budgets, guardrails).
`openclaw-1ly-payments` | OpenClaw-specific setup for using 1ly MCP as the payment layer.
`moltbook-1ly-payments` | Moltbook-specific guidance for monetizing and buying via 1ly.

## Notes

- MCP server package: `@1ly/mcp-server` (npm).
- If a skill depends on another (e.g., `openclaw-1ly-payments` depends on `1ly-payments`), load the core skill first.
