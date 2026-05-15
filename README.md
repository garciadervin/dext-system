# Dext System Agents

![Dext System Agents Banner](https://drive.google.com/uc?export=view&id=1euU0eJkZIzaxTbDZlRXyuXr4W7TZ-tI8)

[![OpenCode](https://img.shields.io/badge/OpenCode-enabled-1f6feb?style=flat&logo=opencollective&logoColor=white)](https://opencode.ai)
[![MCP](https://img.shields.io/badge/MCP-context7%20%26%20obsidian-7c3aed?style=flat&logo=microsoft&logoColor=white)](https://modelcontextprotocol.io)

> *“Simplicity is the ultimate sophistication.”* – Leonardo da Vinci

Spec‑driven OpenCode orchestration with persistent memory and reliable multi‑agent workflows.

## 🚀 Features

- 🧭 **SDD/TDD workflow** – Specifications and backlog first, test‑driven development, phase handoffs.
- 🧪 **Quality gates** – Mandatory pre‑commit checklist (lint, tests, formatting, documentation).
- 🔐 **Security rules** – Non‑negotiable: no secret exposure, no destructive actions without permission.
- 🧠 **Obsidian memory** – Project session notes + reusable learnings, fully linked for continuity.
- 🤝 **Multi‑agent roles** – Orchestrator, Tester, Developer, Reviewer (ISO/IEC 25010 audit).
- 🔌 **MCP integrations** – Context7 (latest library docs) + Obsidian (vault persistence).

## 🧱 Stack

| Component   | Detail |
|-------------|--------|
| Platform    | [OpenCode](https://opencode.ai) |
| Model       | DeepSeek (or any compatible LLM) |
| MCP servers | Context7 (remote) + Obsidian via MCPVault (local) |
| Format      | Markdown (agents, skills) & JSON (config) |

## 🧪 Quick Install

```bash
# 1. Clone the repository
git clone https://github.com/garciadervin/dext-system.git ~/dext-system

# 2. Merge into your OpenCode configuration folder
cp -r ~/dext-system/. ~/.config/opencode

# 3. Remove the temporary clone (optional)
rm -rf ~/dext-system
```

> **Note:** Adjust the Obsidian vault path in `opencode.json` to match your local setup.

## 🧭 How It Works

1. **Orchestrator** – Creates technical spec and backlog, then dispatches phases. Speaks Venezuelan Spanish to the user.
2. **Tester** – Writes failing tests for critical paths using AAA (Arrange‑Act‑Assert). Never touches production code.
3. **Developer** – Implements minimal code to pass tests, adds reasonable improvements (responsive styling, error handling, small refactors), and runs the pre‑commit checklist.
4. **Reviewer** – Performs a read‑only audit based on ISO/IEC 25010 (optional, on demand).

All handoffs, code, specs, and memory notes are in **English**. Only the user‑facing chat uses **Venezuelan Spanish**. Sessions and learnings are stored automatically in your Obsidian vault for long‑term continuity.

## 🗂️ Project Structure

```
.
├── agents/                 # Dext roles
│   ├── dext-developer.md
│   ├── dext-orchestrator.md
│   ├── dext-reviewer.md
│   └── dext-tester.md
├── skills/                 # Optional skills
│   ├── agent-browser/
│   ├── architecture-patterns/
│   ├── code-reviewer/
│   ├── frontend-design/
│   ├── gh-cli/
│   ├── seo-audit/
│   ├── supabase/
│   ├── vercel-react-best-practices/
│   ├── vercel-react-native-skills/
│   └── webapp-testing/
├── AGENTS.md               # Full constitution and rules
├── README.md               # This file
└── opencode.json           # OpenCode configuration
```

> This is a **configuration bundle** – copy the entire contents into your OpenCode folder to activate the system.

## 📜 License

Proprietary. All rights reserved.