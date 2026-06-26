# My Personal Agent Skills

This repository contains my personal collection of custom **skills** for my AI coding assistant (Gemini/Antigravity). These skills extend the capabilities of the agent, providing it with specialized instructions and workflows for a variety of complex tasks.

## 🚀 Overview of Skills

Here are some of the skills included in this repository:

* **Design & Diagrams**: `architecture-diagram`, `concept-diagrams`, `popular-web-designs`
* **Workflow & Planning**: `grill-me`, `grill-with-docs`, `make-todo`, `to-issues`, `to-prd`, `triage`, `zoom-out`
* **Coding & Architecture**: `tdd`, `diagnose`, `improve-codebase-architecture`, `karpathy-guidelines`, `prototype`
* **Agent Utility**: `caveman`, `handoff`, `lean-ctx`, `setup-matt-pocock-skills`, `write-a-skill`
* **Creative & Fun**: `ascii-art`, `pixel-art`, `humanizer`, `godmode`

## 📁 Structure

Each skill is located in its own directory and contains a core `SKILL.md` file. This markdown file holds the YAML frontmatter (name, description) which triggers the skill when I mention related topics, along with the detailed markdown instructions the agent follows when the skill is activated.

More complex skills may also contain supplementary scripts or examples within their directory.

## ⚙️ Usage

Because these are located in my standard `skills` customizations root (`.gemini/skills`), my agent will automatically discover and load them without any manual registration required. When I give the agent a task relevant to one of these skills, it will automatically pull in the associated instructions!
