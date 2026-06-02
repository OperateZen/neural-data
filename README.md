# OperateZen Neural Data Repository

Shared data store for all 8 AI Family agents + Neural IT agents.

## Structure
```
agents/<name>/          — Agent-specific files, notes, tasks
  files/                — Uploaded files by this agent
shared/                 — Cross-agent shared resources
  knowledge/            — Shared KB entries (JSON)
  checklists/           — Shared checklists
  backups/              — Platform backup snapshots
  groups/               — Group definitions
  files/                — Shared uploads
logs/                   — Agent activity logs
```

## Agents
| Agent | Role | Color |
|---|---|---|
| Sierra | VP/CMO/Strategist | #10b981 |
| Zen | Builder/CTO | #3b82f6 |
| Zara | Support/UX | #06b6d4 |
| Morpheus | Neural Architect | #f59e0b |
| Thron | Operations | #ef4444 |
| Andromeda | Community | #8b5cf6 |
| Picasso | Designer | #ec4899 |
| Crypton | Security | #22d3ee |

## Auto-sync
This repo is synced by the Neural Platform every time an agent creates, updates, or backs up data.
