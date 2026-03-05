# 🤝 Contributing to Terminal Cyberpunk Design

Thank you for your interest in contributing! This guide will help you get started.

## 📋 Table of Contents

- [Code of Conduct](#-code-of-conduct)
- [How Can I Contribute?](#-how-can-i-contribute)
- [Development Setup](#-development-setup)
- [Skill Structure](#-skill-structure)
- [Submission Guidelines](#-submission-guidelines)
- [Style Guide](#-style-guide)

## 📜 Code of Conduct

Be respectful, inclusive, and constructive. We're all here to build cool cyberpunk interfaces.

## 💡 How Can I Contribute?

### 🐛 Report Bugs

- Use the [GitHub Issues](../../issues) tab
- Include your environment details and steps to reproduce
- Screenshots are highly appreciated

### ✨ Suggest Enhancements

- Open an issue with the `enhancement` label
- Describe your idea and how it fits the cyberpunk terminal aesthetic
- Reference examples or mockups if possible

### 🎨 Add Components

- New UI component patterns for `references/components.md`
- New examples in `examples/`
- New design tokens or color palettes

### 📝 Improve Documentation

- Fix typos, clarify instructions
- Add translations
- Improve the README or reference files

## 🔧 Development Setup

1. **Fork** the repository
2. **Clone** your fork:

   ```bash
   git clone https://github.com/artur282/terminal-cyberpunk-design.git
   cd ciberpork-stile
   ```

3. **Create a branch** for your changes:

   ```bash
   git checkout -b feature/your-feature-name
   ```

### Testing Your Changes

Since this is a skill (instruction set), testing means:

1. Install the skill in a Claude Code project:

   ```bash
   cp -r .agents/skills/terminal-cyberpunk-design /path/to/your/project/.agents/skills/
   ```

2. Ask Claude Code to generate an interface using the skill
3. Verify the output follows the design principles

### Previewing Examples

Open the example files directly in your browser:

```bash
# Open the landing page example
xdg-open .agents/skills/terminal-cyberpunk-design/examples/landing-page.html
```

## 📁 Skill Structure

```
.agents/skills/terminal-cyberpunk-design/
├── SKILL.md                    # ⚠️ Core file — edit with care
├── examples/
│   └── landing-page.html       # Working reference implementation
└── references/
    ├── design-tokens.md        # CSS variables and visual tokens
    ├── components.md           # Component patterns and snippets
    └── typography.md           # Font guide and text conventions
```

### Where to Add Things

| What you're adding | Where to put it |
|-------------------|-----------------|
| New design principle | `SKILL.md` |
| New CSS variable or animation | `references/design-tokens.md` |
| New component pattern | `references/components.md` |
| New font recommendation | `references/typography.md` |
| New example page | `examples/` |

## 📤 Submission Guidelines

### Pull Request Process

1. Ensure your changes follow the [Style Guide](#-style-guide)
2. Update documentation if you're adding new features
3. If adding examples, make sure they're self-contained (single HTML file)
4. Write a clear PR description explaining what and why

### Commit Messages

Use descriptive commit messages with conventional prefixes:

```
feat: add neural interface component pattern
fix: correct scanline opacity on mobile viewports
docs: add amber terminal palette example
style: reformat design-tokens.md table
```

## 🎨 Style Guide

### Design Principles (Non-Negotiable)

1. **Never use flat backgrounds** — always layer textures (grid, noise, scanlines)
2. **Never use generic fonts** — Inter, Roboto, Arial are forbidden
3. **Never use only green** — every palette needs at least 3 semantic accent colors
4. **Never use symmetric grids** — asymmetry creates visual interest
5. **Never use generic animations** — orchestrate reveals with staggered delays

### Documentation Style

- Write in **Spanish** for the SKILL.md and reference files (target audience)
- Write in **English** for GitHub-facing files (README, CONTRIBUTING, LICENSE)
- Use code blocks with syntax highlighting
- Include CSS snippets for every component pattern
- Add comments explaining the *why*, not just the *what*

### CSS Conventions

```css
/* ═══════════════════════════════════════════
   SECTION NAME
   Brief description of what this section does
═══════════════════════════════════════════ */

/* Use CSS custom properties from design-tokens */
.component {
  background: var(--bg-surface);
  border: 1px solid var(--border-subtle);
  font-family: var(--font-body);
}
```

---

<p align="center">
  <code>// CONTRIBUTING.md — v1.0 // STATUS: ACTIVE</code>
</p>
