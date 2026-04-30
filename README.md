# Dext System Agents

![Dext System Agents Banner](https://drive.google.com/uc?export=view&id=1euU0eJkZIzaxTbDZlRXyuXr4W7TZ-tI8)

![OpenCode](https://img.shields.io/badge/OpenCode-enabled-1f6feb?style=flat&logo=opencollective&logoColor=white)
![MCP](https://img.shields.io/badge/MCP-context7%20%26%20obsidian-7c3aed?style=flat&logo=microsoft&logoColor=white)

Spec-driven OpenCode orchestration with persistent memory and reliable multi-agent workflows.

## 🚀 Features

- 🧭 SDD/TDD workflow with clear specs, backlog, and phase handoffs
- 🧪 Pre-commit quality checklist for tests, lint, and docs
- 🔐 Safety rules for secrets and destructive actions
- 🧠 Obsidian memory for project sessions and learnings
- 🤝 Multi-agent roles: orchestrator, tester, developer, reviewer
- 🔌 MCP integrations for Context7 (remote) and Obsidian (local)

## 🧱 Stack

- **Platform:** OpenCode configuration (`opencode.json`)
- **Models:** `github-copilot/gpt-5.2-codex`, `github-copilot/gpt-5.4-mini`
- **MCP:** Context7 (remote) + Obsidian via `@bitbonsai/mcpvault` (local)
- **Format:** Markdown + JSON

## 🧪 Local Development

```bash
# 1. Clone the repository to a temporary location
git clone https://github.com/garciadervin/dext-system.git ~/dext-system

# 2. Copy the content to your OpenCode folder
# This will merge/overwrite files without deleting the existing folder
cp -r ~/dext-system/. ~/.config/opencode

# 3. Clean up the temporary folder (optional)
rm -rf ~/dext-system
```

> **Note:** Keep `opencode.json` at the repo root and update the Obsidian vault path if needed.

## 🧭 Workflow

- Start with the orchestrator to create specs and backlog.
- Follow the developer checklist for tests, linting, and documentation.
- Use Spanish for user-facing chat and English for technical artifacts.
- Store sessions and learnings in the Obsidian vault for continuity.

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
├── opencode.json
```

> **Note:** This repository is a configuration bundle. Copy its contents into your OpenCode folder to use it.

## 📜 License

Proprietary. All rights reserved.
