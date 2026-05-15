# Dext System Agents

![Dext System Agents Banner](https://drive.google.com/uc?export=view&id=1euU0eJkZIzaxTbDZlRXyuXr4W7TZ-tI8)

[![OpenCode](https://img.shields.io/badge/OpenCode-enabled-1f6feb?style=flat&logo=opencollective&logoColor=white)](https://opencode.ai)
[![MCP](https://img.shields.io/badge/MCP-context7%20%26%20obsidian-7c3aed?style=flat&logo=microsoft&logoColor=white)](https://modelcontextprotocol.io)

> *“Simplicity is the ultimate sophistication.”* – Leonardo da Vinci

Spec-driven OpenCode orchestration with persistent memory and reliable multi-agent workflows.

## 🚀 Features

- 🧭 **SDD/TDD workflow** – specs, backlog, phase handoffs, and test-first development.
- 🧪 **Quality gates** – pre-commit checklist covering tests, lint, formatting, and documentation.
- 🔐 **Security rules** – non-negotiable protection of secrets and destructive actions.
- 🧠 **Obsidian memory** – project session notes and reusable learnings, fully linked.
- 🤝 **Multi-agent roles** – orchestrator, tester, developer, reviewer (ISO/IEC 25010).
- 🔌 **MCP integrations** – Context7 (latest library docs) & Obsidian (vault persistence).

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

1. **Orchestrator** creates technical spec and backlog, then dispatches phases.  
2. **Tester** writes failing tests for critical paths (AAA pattern).  
3. **Developer** implements production code, adds improvements, and runs pre-commit checks.  
4. **Reviewer** performs a read-only audit based on ISO/IEC 25010 (optional, on demand).

All handoffs, code, specs, and memory notes are in **English**. Only the user-facing chat uses **Venezuelan Spanish**. Sessions and learnings are stored automatically in your Obsidian vault for long-term continuity.

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