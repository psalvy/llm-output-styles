# Claude Code Output Style Locations

Claude Code stores output styles in specific local configuration and markdown files depending on whether they are personal or project-wide:

## File Locations

* **Personal Output Styles** (Applies to all projects on your machine):  
  `~/.claude/output-styles/<name>.md`
  
* **Project-Level Output Styles** (Shared with your team in a repository):  
  `.claude/output-styles/<name>.md` (located in the root directory of your project)

* **Active Style Settings**:  
  Your selected active style is saved inside `.claude/settings.local.json` (or managed via the `/config` command).

---

## 🛠️ Custom Style File Structure

Custom output styles are written in Markdown and include YAML frontmatter. Below is an example structure:

```yaml
---
name: custom-style-name
description: A brief description of your custom output style.
keep-coding-instructions: true
---
```

## ⚙️ How to Manage Styles

You can view, manage, or change active styles inside the CLI by running:
```bash
/config
```
Then select **Output style** from the configuration menu.
