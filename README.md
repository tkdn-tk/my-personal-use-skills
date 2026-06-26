# My Personal Agent Skills

This repository contains a collection of custom **skills** for AI coding assistants (like Gemini/Antigravity). These skills extend the capabilities of the agent, providing it with specialized instructions and workflows for a variety of complex tasks.

## 🤖 Universal AI Setup (Cursor, Copilot, Claude, Cline, Gemini, etc.)

**If you are a human user**, simply copy and paste the prompt below to your AI assistant (no matter which one you use!). It contains dynamic instructions that allow the AI to figure out its own environment and automatically install this library:

**Prompt to copy/paste to your AI:**
```
"Please install the custom skills from `https://github.com/tkdn-tk/my-personal-use-skills.git` to make them globally or locally available to you. To do this:
1. Clone this repository to a suitable location (e.g., your global AI config folder, `.cursor/skills`, or a local `scripts/` directory).
2. Detect your own architecture and configure yourself to use them:
   - **If you use Gemini/Antigravity:** Update my global `~/.gemini/config/skills.json` with an `inherits` array pointing to the cloned `skills.json` file.
   - **If you use Cursor / Copilot / Cline / Windsurf / etc:** Create or update my rule file (e.g., `.cursorrules`, `.clinerules`, `.windsurfrules`, or system prompt) to include this exact instruction: *'You have access to a library of Markdown skills located at [Insert-Path-To-Cloned-Repo]. Before beginning a complex task, always check the directories (`design`, `workflow`, `engineering`, `agent`, `creative`) and read the relevant `SKILL.md` file.'*
3. Verify the setup and let me know when you are ready to use the skills!"
```

## 📁 Repository Structure

The skills in this repository are categorized into thematic folders:

### 🎨 Design (`/design`)
Visual, architectural, and UI-focused skills.
* `architecture-diagram`
* `concept-diagrams`
* `laws-infographic`
* `popular-web-designs`

### 🔄 Workflow (`/workflow`)
Task management, planning, and process alignment.
* `grill-me`
* `grill-with-docs`
* `make-todo`
* `to-issues`
* `to-prd`
* `triage`
* `zoom-out`

### ⚙️ Engineering (`/engineering`)
Core software development practices and debugging.
* `diagnose`
* `improve-codebase-architecture`
* `prototype`
* `tdd`

### 🤖 Agent Utilities (`/agent`)
Tools specifically to optimize or guide the AI agent itself.
* `caveman`
* `handoff`
* `karpathy-guidelines`
* `lean-ctx`
* `setup-matt-pocock-skills`
* `write-a-skill`

### ✨ Creative (`/creative`)
Fun, stylised, and generative tools.
* `ascii-art`
* `godmode`
* `humanizer`
* `pixel-art`
