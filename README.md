# Dext System Agents

![Dext System Agents Banner](https://drive.google.com/uc?export=view&id=1euU0eJkZIzaxTbDZlRXyuXr4W7TZ-tI8)

![OpenCode](https://img.shields.io/badge/OpenCode-enabled-1f6feb?style=flat&logo=opencollective&logoColor=white)
![MCP](https://img.shields.io/badge/MCP-context7%20%26%20obsidian-7c3aed?style=flat&logo=microsoft&logoColor=white)

Spec-driven OpenCode orchestration with persistent memory and reliable multi-agent workflows.

## 🚀 Features

- 🧭 **SDD/TDD workflow**: technical specs, product backlog, and phase‑based handoffs
- 🧪 **Pre‑commit quality**: linting, type checking, tests, and docs before every commit
- 🔐 **Security first**: secrets and destructive actions are explicitly blocked or need approval
- 🧠 **Obsidian memory**: permanent project sessions and cross‑project learnings
- 🤝 **Multi‑agent roles**: orchestrator, tester, developer, reviewer – each with clear boundaries
- 🔌 **MCP integrations**: Context7 (real‑time library docs) + Obsidian (local knowledge base)

## 🧱 Stack

- **Platform:** OpenCode (`opencode.json`)
- **Model:** `deepseek/deepseek-v4-flash`
- **MCP:** Context7 (remote) + Obsidian via `@bitbonsai/mcpvault` (local)
- **Format:** Markdown + JSON

## 🧪 Local Development

```bash
# 1. Clone the repository to a temporary location
git clone https://github.com/garciadervin/dext-system.git ~/dext-system

# 2. Copy its contents into your OpenCode configuration folder
#    (adjust the destination if your OpenCode directory differs)
cp -r ~/dext-system/. ~/.config/opencode/

# 3. Clean up the temporary clone (optional)
rm -rf ~/dext-system
```

> **Important:**  
> - The `opencode.json` file is kept at the repo root; it expects to sit directly inside your OpenCode folder.  
> - After copying, open `opencode.json` and update the Obsidian vault path to match your local setup.

## 🧭 Workflow

1. The **orchestrator** creates the spec and product backlog, then dispatches phases.
2. The **tester** writes minimal failing tests based on the spec.
3. The **developer** implements the code to pass all tests, adds UI polish, and runs the pre‑commit checklist.
4. The **reviewer** performs a final read‑only audit (on demand) using ISO/IEC 25010.
5. All technical output is in English; the user‑facing chat uses Venezuelan Spanish.
6. Every session and important finding is stored in the Obsidian vault for long‑term memory.

## 🗂️ Structure

```
.
├── agents/
│   ├── dext-developer.md
│   ├── dext-orchestrator.md
│   ├── dext-reviewer.md
│   └── dext-tester.md
├── skills/
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
├── AGENTS.md
├── README.md
└── opencode.json
```

> **Note:** This repository is a configuration bundle. Copy its contents into your OpenCode folder to activate the agents.

## 📜 License

Proprietary. All rights reserved.