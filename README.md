# 🚀 ShellCraft

<div align="center">

![ShellCraft](https://img.shields.io/badge/ShellCraft-tmux-845EC2?style=for-the-badge&logo=tmux&logoColor=white)
![Version](https://img.shields.io/badge/version-1.0.0-ff8066?style=for-the-badge)
![License](https://img.shields.io/badge/license-MIT-4e8397?style=for-the-badge)

**Professional, Modular Tmux Configuration Framework**

*Elegant • Customizable • Powerful*

</div>

---

## ✨ Features

- 🎨 **Full Hex Color Support** - True color RGB/Hex palette
- ⚡ **Visual Prefix Indicator** - Know when prefix is active
- 📋 **Enhanced Copy Mode** - Step-by-step visual feedback
- 🎯 **Modular Architecture** - Easy to customize and extend
- 🪟 **Clean Status Bar** - Minimal, elegant design
- ⌨️ **Vim-style Navigation** - Familiar keybindings
- 🌈 **5 Built-in Color Presets** - Switch themes instantly
- 💡 **Interactive Help Menu** - Fully colorized reference

---

## 📦 Installation
```bash
# Clone or download the install script
bash install_script.sh
```

### Directory Structure
```
~/.dotfiles/tmux/
├── .tmux.conf                    # Main entry point
└── .config/core/
    ├── colors.conf               # Color customization
    ├── settings.conf             # Performance settings
    ├── keybindings.conf          # All keybindings
    ├── panes.conf                # Pane styling
    ├── windows.conf              # Window management
    └── statusbar.conf            # Status bar config
```

---

## ⚡ Quick Start

### Essential Keybindings

| Keybinding | Action |
|------------|--------|
| `Ctrl+s` | **Prefix Key** |
| `Ctrl+s + ?` | Show help menu |
| `Ctrl+s + r` | Reload configuration |
| `Ctrl+s + 9` | Split vertically |
| `Ctrl+s + 0` | Split horizontally |
| `Ctrl+s + h/j/k/l` | Navigate panes (vim-style) |
| `Ctrl+s + [` | Enter copy mode |
| `v` (in copy mode) | Start selection |
| `y` (in copy mode) | Copy selection |
| `Ctrl+s + ]` | Paste |

---

## 🎨 Customization

### Changing Colors

Edit `~/.dotfiles/tmux/.config/core/colors.conf`:
```bash
# Main status bar background
TMUX_STATUS_BG="#4b4453"

# Active window highlight
TMUX_ACTIVE_WINDOW_BG="#845ec2"

# Prefix indicator (when Ctrl+s pressed)
TMUX_PREFIX_ACTIVE_BG="#ff8066"

# Window boxes background
TMUX_WINDOW_BOX_BG="#7c57ba"
```

**Apply changes:**
```bash
# Press in tmux
Ctrl+s + r
```

### Built-in Color Presets

Uncomment a preset in `colors.conf`:

1. **Purple Dream** (default) - `#845ec2`
2. **Ocean Breeze** - `#4e8397`
3. **Magenta Vibe** - `#be36b3`
4. **Coral Sunset** - `#ff8066`
5. **Teal Professional** - `#2c3e50`

---

## 📋 Copy Mode Guide

ShellCraft enhances copy mode with visual feedback:

1. **Enter Copy Mode**: `Ctrl+s + [`
   - Status bar shows: `📋 COPY MODE`
   - Message: *"Press 'v' to select, 'y' to copy"*

2. **Start Selection**: Press `v`
   - Message: *"✓ Selection Started | Press 'y' to copy"*

3. **Copy Text**: Press `y`
   - Message: *"✓ Copied! | Use Ctrl+s + ] to paste"*

4. **Paste**: `Ctrl+s + ]`
   - Message: *"✓ Pasted from buffer"*

---

## 🔧 Configuration Options

### Message Display Time

Edit `~/.dotfiles/tmux/.config/core/settings.conf`:
```bash
# Display messages for 3 seconds (3000ms)
set -g display-time 3000
```

### Enable True Color Support

Add to your `~/.bashrc` or `~/.zshrc`:
```bash
export COLORTERM=truecolor
```

---

## 🎯 Advanced Features

### Pane Management
- Vim-style navigation: `h`, `j`, `k`, `l`
- Resize panes: `H`, `J`, `K`, `L` (repeatable)
- Break pane to window: `Ctrl+s + b`

### Window Management
- Create new window: `Ctrl+s + c`
- Previous window: `Ctrl+s + Ctrl+h`
- Next window: `Ctrl+s + Ctrl+l`

### Status Bar Features
- **Prefix Indicator**: Shows `⚡` when active
- **Copy Mode Badge**: Shows `📋 COPY MODE` when active
- **Session Name**: Current session displayed
- **Help Hint**: Always visible shortcut

---

## 🐛 Troubleshooting

### Colors not showing correctly?
```bash
# Check terminal support
echo $COLORTERM  # Should show 'truecolor'

# Add to shell config
export COLORTERM=truecolor
```

### Changes not applying?
```bash
# Reload tmux configuration
Ctrl+s + r

# Or from command line
tmux source ~/.tmux.conf
```

### Prefix key not working?
Check if another program is using `Ctrl+s`. You can change the prefix in `keybindings.conf`.

---

## 🤝 Contributing

Contributions are welcome! Feel free to:
- Report bugs
- Suggest features
- Submit pull requests
- Share your color presets

---

## 📝 License

MIT License - Free to use and modify

---

## 👨‍💻 Author

**penguinshero**

- GitHub: [@penguinshero](https://github.com/penguinshero)
- Ethical hacker & technology explorer

---

## 🌟 Show Your Support

If you find ShellCraft useful, give it a ⭐️ on GitHub!

---

<div align="center">

**Made with ❤️ by penguinshero**

*ShellCraft - Terminal multiplexing, elevated.*

</div>

