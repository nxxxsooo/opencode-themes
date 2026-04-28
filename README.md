<p align="center">
  <img src="obsidian/screenshot.png" alt="OpenCode Themes" width="600" />
</p>

<h1 align="center">OpenCode Themes</h1>

<p align="center">
  <strong>Terminal-inspired dark themes for <a href="https://obsidian.md">Obsidian</a>, <a href="https://typora.io">Typora</a>, and <a href="https://ghostty.org">Ghostty</a>.</strong><br/>
  Deep blacks · Precise contrast · Built for focus.
</p>

<p align="center">
  <a href="https://mjshao.fun/opencode-themes/"><img src="https://img.shields.io/badge/🌐_Landing_Page-Visit-8a6cc4?style=flat-square" alt="Landing Page" /></a>
  <a href="LICENSE"><img src="https://img.shields.io/github/license/nxxxsooo/opencode-themes?style=flat-square&color=5fd4bb" alt="License" /></a>
  <a href="https://github.com/nxxxsooo/opencode-themes/stargazers"><img src="https://img.shields.io/github/stars/nxxxsooo/opencode-themes?style=flat-square&color=f0a830" alt="Stars" /></a>
</p>

---

## Design Philosophy

> Write in the dark. Focus on the code.

OpenCode Themes bring the terminal to your writing tools — deep blacks, precise contrast, and a palette tuned for extended reading and writing sessions. Inspired by [OpenCode](https://github.com/sst/opencode) and [Ghostty](https://ghostty.org) terminal aesthetics.

---

## Editors

| Editor | Status | Source |
|--------|--------|--------|
| <img src="https://img.shields.io/badge/Obsidian-d19af8?style=flat-square&logo=obsidian&logoColor=white" /> | ✅ Published to Community Themes | [`obsidian/`](obsidian/) · [Standalone Repo](https://github.com/nxxxsooo/obsidian-opencode-theme) |
| <img src="https://img.shields.io/badge/Typora-5fd4bb?style=flat-square" /> | ✅ Ready | [`typora/`](typora/) |
| <img src="https://img.shields.io/badge/Ghostty-fab283?style=flat-square" /> | ✅ Ready | [`ghostty/`](ghostty/) |

---

## Color Palette

| | Element | Hex | Role |
|---|---------|-----|------|
| 🟠 | **Primary / Cursor** | `#fab283` | Links, cursor, primary actions |
| 🟣 | **Accent** | `#9d7cd8` | Headings, keywords |
| 🔵 | **Secondary** | `#5c9cf5` | Lists, focused states |
| 🟢 | **Green** | `#7fd88f` | Strings, success |
| 🟡 | **Yellow** | `#e5c07b` | Emphasis, warnings |
| 🟠 | **Orange** | `#f5a742` | Strong text, numbers |
| 🔴 | **Red** | `#e06c75` | Errors, deletions |
| 🩵 | **Cyan** | `#56b6c2` | Operators, tags, info |
| ⬛ | **Background** | `#0a0a0a` | Deep black base |
| ◼️ | **Panel** | `#141414` | Secondary surfaces |
| ⬜ | **Text** | `#eeeeee` | High contrast foreground |

---

## Features

#### ⌨️ Terminal-First Design
Color scheme derived from OpenCode/Ghostty terminal — feels native to developers.

#### 👁️ High Contrast
`#eeeeee` on `#0a0a0a` — optimized for readability in dark environments.

#### 📝 Full Syntax Highlighting
Complete token coverage — keywords, strings, functions, properties, operators all precisely colored.

#### 🖨️ Print Ready (Typora)
Clean light export for PDF and print output.

#### 🎨 Accent Customizable (Obsidian)
Override the purple accent via **Settings → Appearance → Accent Color**.

#### 🀄 CJK Optimized
PingFang SC / Noto Sans SC for beautiful Chinese/Japanese/Korean text.

---

## Installation

### Obsidian

**From Community Themes:**

1. Open **Settings** → **Appearance** → **Themes**
2. Click **Manage** → **Browse**
3. Search for `OpenCode`
4. Click **Install and use**

**Manual:**

1. Download [`theme.css`](obsidian/theme.css) and [`manifest.json`](obsidian/manifest.json)
2. Create folder: `{vault}/.obsidian/themes/OpenCode/`
3. Place both files in the folder
4. Enable in **Settings** → **Appearance** → **Themes**

### Typora

1. Download [`opencode.css`](typora/opencode.css)
2. Open Typora → **Preferences** → **Appearance** → **Open Theme Folder**
3. Copy `opencode.css` into the theme folder
4. Restart Typora and select **OpenCode** from the theme menu

### Ghostty

1. Download [`OpenCode`](ghostty/OpenCode)
2. Copy it into your Ghostty user themes folder:
   ```bash
   mkdir -p ~/.config/ghostty/themes
   cp OpenCode ~/.config/ghostty/themes/OpenCode
   ```
3. Add this to `~/.config/ghostty/config`:
   ```conf
   theme = dark:OpenCode,light:Aura
   ```
4. Reload Ghostty with `Cmd + Shift + ,` or restart it.

### 🤖 For AI Agents (One-liner)

```bash
# Obsidian
VAULT="$(find ~/Library/Application\ Support/obsidian -name '.obsidian' -maxdepth 3 2>/dev/null | head -1)" && \
mkdir -p "$VAULT/themes/OpenCode" && \
curl -sL https://raw.githubusercontent.com/nxxxsooo/obsidian-opencode-theme/main/theme.css -o "$VAULT/themes/OpenCode/theme.css" && \
curl -sL https://raw.githubusercontent.com/nxxxsooo/obsidian-opencode-theme/main/manifest.json -o "$VAULT/themes/OpenCode/manifest.json" && \
echo "✅ Obsidian OpenCode theme installed"

# Typora
TYPORA_THEMES="$(find ~/Library/Application\ Support/abnerworks.Typora/themes -maxdepth 0 2>/dev/null || echo '')" && \
[ -n "$TYPORA_THEMES" ] && \
curl -sL https://raw.githubusercontent.com/nxxxsooo/opencode-themes/main/typora/opencode.css -o "$TYPORA_THEMES/opencode.css" && \
echo "✅ Typora OpenCode theme installed"

# Ghostty
mkdir -p "$HOME/.config/ghostty/themes" && \
curl -sL https://raw.githubusercontent.com/nxxxsooo/opencode-themes/main/ghostty/OpenCode -o "$HOME/.config/ghostty/themes/OpenCode" && \
grep -q '^theme = ' "$HOME/.config/ghostty/config" 2>/dev/null \
  && perl -0pi -e 's/^theme = .*$/theme = dark:OpenCode,light:Aura/m' "$HOME/.config/ghostty/config" \
  || printf '\ntheme = dark:OpenCode,light:Aura\n' >> "$HOME/.config/ghostty/config" && \
echo "✅ Ghostty OpenCode theme installed"
```

> macOS paths shown. On Linux/Windows, adjust vault/theme folder paths accordingly.

---

## Typography

| Element | Font |
|---------|------|
| Body text | PingFang SC, system sans-serif |
| Code | JetBrains Mono, Fira Code, Cascadia Code |
| Display (web) | Space Grotesk |

> **Tip**: Install [JetBrains Mono](https://www.jetbrains.com/lp/mono/) for the best code block experience.

---

## Repository Structure

```
opencode-themes/
├── obsidian/           # Obsidian theme
│   ├── theme.css       # Main theme stylesheet
│   ├── manifest.json   # Obsidian manifest
│   └── screenshot.png  # Theme preview
├── typora/             # Typora theme
│   ├── opencode.css    # Main theme stylesheet
│   └── opencode/       # Asset folder (fonts/images)
├── ghostty/            # Ghostty terminal theme
│   └── OpenCode        # Ghostty user theme file
├── website/            # Landing page
│   └── index.html      # Static site for GitHub Pages
└── README.md
```

---

## Credits

- Terminal aesthetic from [OpenCode](https://github.com/sst/opencode)
- Font rendering tuned for [Ghostty](https://ghostty.org)
- README format inspired by [Bloom Theme](https://github.com/webkubor/typora-Bloom-theme)

---

## License

[MIT](LICENSE) © [nxxxsooo](https://github.com/nxxxsooo)
