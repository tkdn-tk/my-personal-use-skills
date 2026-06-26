# My Personal Agent Skills

This repository contains my personal collection of custom **skills** for my AI coding assistant (Gemini/Antigravity). These skills extend the capabilities of the agent, providing it with specialized instructions and workflows for a variety of complex tasks.

## 📁 Repository Structure

The skills in this repository are categorized into thematic folders to keep everything organized:

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

## ⚙️ Usage Configuration

Because the skills are now grouped into sub-folders, you will need to map them in your global `skills.json` file so your agent can discover them. 

Add the following to your `C:\Users\injec\.gemini\config\skills.json`:

```json
{
  "entries": [
    { "path": "C:\\Users\\injec\\.gemini\\skills\\design" },
    { "path": "C:\\Users\\injec\\.gemini\\skills\\workflow" },
    { "path": "C:\\Users\\injec\\.gemini\\skills\\engineering" },
    { "path": "C:\\Users\\injec\\.gemini\\skills\\agent" },
    { "path": "C:\\Users\\injec\\.gemini\\skills\\creative" }
  ]
}
```
