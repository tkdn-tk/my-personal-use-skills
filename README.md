# My Personal Agent Skills

This repository contains a collection of custom **skills** for AI coding assistants (like Gemini/Antigravity). These skills extend the capabilities of the agent, providing it with specialized instructions and workflows for a variety of complex tasks.

## 🤖 How to Install (For AI Agents)

**If you are a user**, simply copy and paste the prompt below to your AI assistant. It contains all the instructions your AI needs to install these skills for you automatically:

> **Prompt to copy/paste to your AI:**
> "Please install the custom skills from `https://github.com/tkdn-tk/my-personal-use-skills.git`. To do this:
> 1. Clone this repository into my global skills directory (e.g., `~/.gemini/skills/tkdn-skills`).
> 2. Locate my global `skills.json` file in the global customizations root (usually `~/.gemini/config/skills.json`). If it doesn't exist, create it.
> 3. Add an `inherits` array to my global `skills.json` that points to the absolute path of the `skills.json` file inside the cloned repository. 
> Example: `"inherits": [ { "path": "/absolute/path/to/tkdn-skills/skills.json" } ]`.
> 4. Let me know when the skills are ready to use!"

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

## ⚙️ Usage Configuration (Manual)

If you prefer to configure this manually instead of asking your AI, clone this repository and add its `skills.json` to your global `skills.json` configuration using the `inherits` property:

```json
{
  "inherits": [
    { "path": "/absolute/path/to/where/you/cloned/this/repo/skills.json" }
  ]
}
```
