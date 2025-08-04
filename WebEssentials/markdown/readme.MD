# 📝 Markdown Quick Reference & Notes

This file contains concise notes, syntax examples, quirks, and tools related to Markdown. It’s designed for developers, content creators, and anyone working with documentation, READMEs, or static site generators.

> ✅ Best viewed on GitHub or a Markdown viewer with code highlighting.

---

## 📌 What is Markdown?

Markdown is a lightweight markup language used to format plain text into HTML. Common use cases include:

- GitHub README and docs
- Static site generators (Docsify, Docusaurus, Jekyll)
- Blogging platforms (Dev.to, Hashnode)
- Note-taking (Obsidian, Notion export)
- PDF and documentation exports

---

## ⚙️ Core Syntax

| Element         | Syntax               | Output                       |
| --------------- | -------------------- | ---------------------------- |
| Heading         | `# H1` → `###### H6` | # H1 to ###### H6            |
| Bold            | `**text**`           | **text**                     |
| Italic          | `*text*`             | _text_                       |
| Bold + Italic   | `***text***`         | **_text_**                   |
| Strikethrough   | `~~text~~`           | ~~text~~                     |
| Blockquote      | `> quote`            | > quote                      |
| Unordered list  | `- item`             | • item                       |
| Ordered list    | `1. item`            | 1. item                      |
| Inline code     | `` `code` ``         | `code`                       |
| Code block      | `js\ncode\n`         | See below                    |
| Link            | `[label](url)`       | [Google](https://google.com) |
| Image           | `![alt](url)`        | 🖼️                           |
| Horizontal Rule | `---`                | —                            |

---

## 💡 Special Behaviors

### Paragraphs & Line Breaks

- Use **one blank line** to separate paragraphs.
- Use **two spaces at the end of a line** or `<br>` to force a line break.

### Nested Lists

Indent using **4 spaces**:

```md
- Item
  - Subitem
```

### Escaping Characters

Use `\` to escape special symbols:

```md
\*not italic\*
```

### Combining Formatting

```md
**_bold italic_** ← ✅
**_bold italic_** ← ✅
```

---

## 📚 Advanced Features

### ✅ GitHub-Supported

- **Task Lists**:

```md
- [x] Completed Task
- [ ] To-do Item
```

- **Tables**:

```md
| Name | Role |
| ---- | ---- |
| Ashu | Dev  |
```

- **Collapsible Sections**:

```html
<details>
  <summary>Click to expand</summary>

  Hidden content here!
</details>
```

### ❌ Not Supported on GitHub

- Footnotes (`[^1]`)
- LaTeX math (`$E = mc^2$`)
- Definition lists (`Term: Definition`)

---

## 🧠 Common Gotchas

| Issue                             | Explanation                                  |
| --------------------------------- | -------------------------------------------- |
| Single newline doesn't break line | Add two spaces at end or use `<br>`          |
| Code blocks not rendering         | Leave blank lines before and after           |
| Broken lists                      | Needs blank line above list in some cases    |
| Escaping special characters       | Use backslashes: `\* \# \_`                  |
| Platform inconsistencies          | GitHub, VS Code, Obsidian render differently |

---

## 🧰 Markdown Tools & Learning Resources

### 📗 Editors & VS Code Extensions

| Tool                                                                                                  | Purpose                                             |
| ----------------------------------------------------------------------------------------------------- | --------------------------------------------------- |
| [Markdown All in One](https://marketplace.visualstudio.com/items?itemName=yzhang.markdown-all-in-one) | VS Code: live preview, shortcuts, table of contents |
| [Markdown PDF](https://marketplace.visualstudio.com/items?itemName=yzane.markdown-pdf)                | VS Code: export Markdown files to PDF               |
| [Obsidian](https://obsidian.md)                                                                       | Powerful Markdown-based note-taking tool            |

---

### 🧪 Online Editors & Testbeds

| Tool                                                     | Purpose                                                         |
| -------------------------------------------------------- | --------------------------------------------------------------- |
| [Dillinger.io](https://dillinger.io/)                    | Live Markdown editor with export/import options                 |
| [Markdown-It Playground](https://markdown-it.github.io/) | Test Markdown syntax with plugin options                        |
| [StackEdit.io](https://stackedit.io/)                    | Rich online editor with Google Drive sync and advanced features |
| [HackMD.io](https://hackmd.io/)                          | Real-time collaborative Markdown documentation platform         |

---

### 📘 Documentation & Learning

- 📘 **[Markdown Guide](https://www.markdownguide.org/)**
  Beginner to advanced reference with examples, extended syntax, and cheatsheets.

- 🧑‍🏫 **[CommonMark Tutorial](https://commonmark.org/help/tutorial/)**
  Interactive tutorial based on the CommonMark spec (used by most platforms).

- 📖 **[GitHub Flavored Markdown Docs](https://github.github.com/gfm/)**
  GitHub's official reference for supported syntax including task lists, tables, etc.

- 📖 **[CommonMark Spec](https://spec.commonmark.org/)**
  Authoritative technical spec for standardized Markdown syntax.

- 🧠 **[Markdown Cheatsheet by Adam Pritchard](https://github.com/adam-p/markdown-here/wiki/Markdown-Cheatsheet)**
  Great printable all-in-one cheatsheet with code examples.

---

### 🧱 Site Generators & Docs Frameworks

- 📦 **[Docsify](https://docsify.js.org/)**
  Create single-page documentation websites directly from Markdown — no build required.

- 📦 **[Docusaurus](https://docusaurus.io/)**
  Meta’s static site generator for docs using Markdown + React + versioning support.

---

## 🌍 Platform Differences

| Platform        | Engine                         | Notes                                    |
| --------------- | ------------------------------ | ---------------------------------------- |
| GitHub          | GFM (GitHub Flavored Markdown) | Supports tables, checkboxes, code blocks |
| VS Code         | Markdown-It                    | Great preview, supports plugins          |
| Obsidian        | Custom + Markdown-It           | Adds footnotes, backlinks, tags          |
| Dev.to / Jekyll | Kramdown                       | Supports minimal HTML                    |
| Notion          | Proprietary                    | Converts to MD on export, some quirks    |
