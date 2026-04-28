# opencode-themes

## Overview
Monorepo for OpenCode-branded themes across multiple editors and terminals. Contains Obsidian, Typora, Ghostty, and website themes all synced to the OpenCode TUI default palette.

## Architecture
```
opencode-themes/
├── obsidian/          # Obsidian theme (synced copy from obsidian-opencode-theme repo)
│   ├── theme.css
│   ├── manifest.json
│   └── screenshot.png
├── typora/            # Typora theme
│   ├── opencode.css
│   └── opencode/      # (empty, placeholder for font assets)
├── ghostty/           # Ghostty terminal theme
│   └── OpenCode       # Ghostty user theme file
├── website/           # Landing page / showcase
└── README.md
```

## Key Files
- `obsidian/theme.css` — Obsidian theme (MUST stay in sync with obsidian-opencode-theme repo)
- `obsidian/manifest.json` — Version must match obsidian-opencode-theme
- `typora/opencode.css` — Typora dark theme
- `ghostty/OpenCode` — Ghostty terminal theme
- CSS download URL: `https://raw.githubusercontent.com/nxxxsooo/opencode-themes/main/typora/opencode.css`

## Patterns & Conventions
- All themes derive from OpenCode TUI palette: primary=#fab283, accent=#9d7cd8, secondary=#5c9cf5
- The canonical Obsidian theme source is `obsidian-opencode-theme` repo — this repo's `obsidian/` is a sync copy
- Version bumps must happen in BOTH repos simultaneously
- Typora theme submitted to official gallery via PR to typora/theme.typora.io (PR #460, 2026-03-23)
- Ghostty theme can be installed to `~/.config/ghostty/themes/OpenCode` and activated via `theme = dark:OpenCode,light:Aura`

## Related Repos
- `obsidian-opencode-theme` — Obsidian community theme (required separate repo for marketplace)
- `nxxxsooo/theme.typora.io` — Fork of Typora gallery for PR submissions

## Resolved Issues
- v1.3.0: Full palette realignment from Tokyo Night to OpenCode TUI default (opencode.json)
- Typora opencode.css rewritten as proper dark theme with complete palette
