# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Overview

This is a pure VS Code theme extension — no build step, no JavaScript/TypeScript. All themes are JSON files in `themes/`. The extension manifest is `package.json`.

## Publishing

To package and publish to the VS Code Marketplace:

```bash
# Install vsce if not already installed
npm install -g @vscode/vsce

# Package the extension
vsce package

# Publish (requires a PAT configured)
vsce publish
```

Version bumps are done manually in `package.json` and `CHANGELOG.md`.

## Development

To test themes locally, press **F5** in VS Code (uses `.vscode/launch.json`) to open an Extension Development Host window with the themes loaded.

## Architecture

- **`themes/*.json`** — One JSON file per theme. Each file defines:
  - `colors` — VS Code workbench UI colors (sidebar, editor, activity bar, etc.)
  - `tokenColors` — Syntax highlighting rules using TextMate scopes
  - `type` — Either `"light"` or `"dark"` (used by VS Code for icon themes)
  - `uiTheme` in `package.json` — Either `"vs"` (light) or `"vs-dark"` (dark)
- **`package.json`** — Declares all themes under `contributes.themes`. Each entry maps a label, uiTheme, and path to a theme JSON file.
- **`media/`** — Screenshots used in the README and marketplace listing.

## Theme Naming Convention

| File name pattern | Windows era |
|---|---|
| `windows-31-classic.json` | Windows 3.1 |
| `windows-98*.json` | Windows 98 (base + variants: eggplant, desert, rainy-day) |
| `windows-me.json` | Windows ME |
| `windows-xp-{light,dark,blue}.json` | Windows XP |
| `windows-7.json` | Windows 7 |

## Adding a New Theme

1. Create `themes/<name>.json` following the structure of an existing theme.
2. Add an entry to the `contributes.themes` array in `package.json` with the correct `uiTheme` (`"vs"` for light, `"vs-dark"` for dark).
3. Add a preview screenshot to `media/` and reference it in `README.md`.
4. Document the new theme in `CHANGELOG.md`.
