<div align="center">

```
██████╗  ██████╗ ████████╗███████╗██╗██╗     ███████╗███████╗
██╔══██╗██╔═══██╗╚══██╔══╝██╔════╝██║██║     ██╔════╝██╔════╝
██║  ██║██║   ██║   ██║   █████╗  ██║██║     █████╗  ███████╗
██║  ██║██║   ██║   ██║   ██╔══╝  ██║██║     ██╔══╝  ╚════██║
██████╔╝╚██████╔╝   ██║   ██║     ██║███████╗███████╗███████║
╚═════╝  ╚═════╝    ╚═╝   ╚═╝     ╚═╝╚══════╝╚══════╝╚══════╝
```

# 🏔️ My Arch Linux `.config`

### A carefully crafted Hyprland desktop environment setup

![Arch Linux](https://img.shields.io/badge/Arch_Linux-1793D1?style=for-the-badge&logo=arch-linux&logoColor=white)
![Hyprland](https://img.shields.io/badge/Hyprland-58E1FF?style=for-the-badge&logo=wayland&logoColor=black)
![License](https://img.shields.io/badge/License-MIT-green?style=for-the-badge)
![Stars](https://img.shields.io/github/stars/yourusername/dotfiles?style=for-the-badge&color=yellow)

</div>

---

## ⚠️ STOP — Read This First!

> **Before you copy anything**, please understand this:
>
> This config is built for **MY machine**. Your hardware, drivers, and system setup are different from mine.
> Blindly copying configs **can break your desktop** or prevent it from starting entirely.
>
> 🔗 **Always read the [Hyprland Wiki](https://wiki.hyprland.org) first.**
> It is the single most important resource for understanding how everything works.

---

## 📦 What's Inside

| Folder | What It Does |
|--------|-------------|
| `alacritty` | Terminal emulator config (fonts, colors, opacity) |
| `fastfetch` | System info display shown at terminal startup |
| `htop` | Resource monitor layout and colors |
| `hypr` | 🌟 **The main one** — Hyprland window manager config |
| `kitty` | Alternative terminal emulator config |
| `neofetch` | Classic system info fetch config |
| `rofi` | App launcher and menu style |
| `scripts` | Custom shell scripts that power everything together |
| `sddm` | Login screen / display manager theme |
| `starship` | Shell prompt config (the beautiful prompt you see) |
| `thefuck` | Auto-corrects your mistyped terminal commands |
| `waybar` | The status bar at the top/bottom of the screen |
| `yazi` | Terminal file manager config |

---

## 🧭 How To Use This — Step By Step

Think of this like a recipe. Don't skip steps! 🍳

### Step 1 — Install Arch Linux
Make sure you have a working Arch Linux installation first.
Not sure how? → [Arch Installation Guide](https://wiki.archlinux.org/title/installation_guide)

### Step 2 — Read the Hyprland Wiki
This is **not optional**. Spend at least 30 minutes reading:
👉 [https://wiki.hyprland.org](https://wiki.hyprland.org)

Pay special attention to:
- [Getting Started](https://wiki.hyprland.org/Getting-Started/Installation/)
- [Configuring Hyprland](https://wiki.hyprland.org/Configuring/Configuring-Hyprland/)
- [Master Tutorial](https://wiki.hyprland.org/Getting-Started/Master-Tutorial/)

### Step 3 — Install the Required Programs

You need to install the tools before copying their configs. Here's the full list:

```bash
# Core
sudo pacman -S hyprland waybar rofi alacritty kitty sddm

# Extras
sudo pacman -S htop neofetch fastfetch starship yazi

# AUR (use yay or paru)
yay -S thefuck
```

> 💡 **Tip:** Don't know what AUR is? Read this → [AUR Wiki](https://wiki.archlinux.org/title/AUR_helpers)

### Step 4 — Back Up Your Existing Config

Before replacing anything, back up what you already have:

```bash
cp -r ~/.config ~/.config_backup
```

This way, if something breaks, you can restore it easily.

### Step 5 — Clone This Repository

```bash
git clone https://github.com/avinavarcher12/.config.git
cd .config
```

### Step 6 — Copy Configs (One at a Time!)

**Don't copy everything at once.** Copy one folder, test it, then move to the next.

```bash
# Example: Copy only the waybar config first
cp -r waybar ~/.config/waybar
```

Restart that specific program and check if it works before copying the next one.

### Step 7 — Customize for YOUR Machine

Open each config file and look for things like:
- **Monitor names** (like `eDP-1`, `HDMI-A-1`) — yours will be different
- **Font names** — install the fonts I use or change them to yours
- **Keybindings** — change them to what feels right for you
- **Colors** — make it yours!

To find your monitor name, run:
```bash
hyprctl monitors
```

---

## 🔤 Fonts Used

This setup uses these fonts. Install them or the UI may look broken:

```bash
# From official repos
sudo pacman -S ttf-jetbrains-mono-nerd ttf-font-awesome noto-fonts

# Or any Nerd Font from https://www.nerdfonts.com/
```

---

## 🐛 Something Broke?

Don't panic. Here's what to do:

1. **Check the Hyprland log:**
   ```bash
   cat /tmp/hypr/$(ls /tmp/hypr/)/hyprland.log
   ```

2. **Restore your backup:**
   ```bash
   cp -r ~/.config_backup ~/.config
   ```

3. **Ask for help in the right places:**
   - [Hyprland Discord](https://discord.gg/hyprland)
   - [r/hyprland](https://www.reddit.com/r/hyprland/)
   - [Arch Linux Forums](https://bbs.archlinux.org/)

---

## 📸 Screenshots

| Desktop | Terminal | Launcher |
|---------|----------|----------|
| ![soon]() | ![soon]() | ![soon]() |

---

## 🙏 Credits & Inspiration

This config was built by learning from the amazing open-source community.

Big thanks to:
- [Hyprland](https://hyprland.org/) by vaxerski
- [Waybar](https://github.com/Alexays/Waybar)
- [r/unixporn](https://www.reddit.com/r/unixporn/) for endless inspiration

---

## 📜 License

This project is under the [MIT License](LICENSE) — feel free to use, modify, and share. Just give credit. 😊

---

<div align="center">

**Made with ❤️ on Arch Linux**

*"I use Arch, btw"* 🐧

</div>
