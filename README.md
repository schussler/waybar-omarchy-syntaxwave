# 🟣 Waybar Omarchy Syntaxwave Config

A sleek, centralized, and performance-oriented Waybar configuration. This setup was built focusing on a clean developer workflow, featuring system monitoring and media controls with a vibrant deep purple aesthetic inspired by the Syntaxwave/Synthwave '84 palette.

![Waybar Preview](https://img.shields.io/badge/Theme-Syntaxwave-8E00FF?style=for-the-badge)
![Platform](https://img.shields.io/badge/Platform-Arch_Linux-1793D1?style=for-the-badge&logo=arch-linux)
![WM](https://img.shields.io/badge/WM-Hyprland-33ccff?style=for-the-badge)

---
<img width="2558" height="1078" alt="image" src="https://github.com/user-attachments/assets/f4ad817e-dab3-4ed5-bf5f-933e9536855a" />

## ✨ Key Features

- **Centralized Layout** — All modules are grouped in a floating center pill for better focus on UltraWide and large displays.
- **Media Control (MPRIS)** — Full Spotify/Media integration via `playerctl`.
- **Resource Monitoring** — Real-time **CPU** and **RAM** usage indicators.
- **Idle Inhibitor** — Quick toggle (Caffeine mode) to prevent screen sleep.
- **Custom Aesthetics:**
  - Deep Purple accent (`#8E00FF`)
  - Clean "Pill" design with optimized padding and margins
  - High-readability font (JetBrainsMono Nerd Font)

---

## 🛠️ Requirements

Ensure you have the following installed on your Arch system:

```bash
sudo pacman -S waybar playerctl otf-font-awesome ttf-jetbrains-mono-nerd
```

---

## 🚀 Installation & Setup

To get the full visual experience, follow these steps to install the base theme and apply this custom configuration.

### 1. Install the Base Theme (Synthwave '84)

First, install the official Omarchy Synthwave theme to ensure all color variables (`@bg`, `@fg`, etc.) are available:

```bash
git clone https://github.com/omacom-io/omarchy-synthwave84-theme.git /tmp/synthwave-theme && \
cp -rf /tmp/synthwave-theme/* ~/.config/waybar && \
rm -rf /tmp/synthwave-theme
```

### 2. Apply this Custom Configuration

Now, run this command to apply the centralized layout and purple tweaks:

```bash
git clone https://github.com/schussler/waybar-omarchy-syntaxwave.git /tmp/waybar-repo && \
cp -rf /tmp/waybar-repo/* ~/.config/waybar && \
rm -rf /tmp/waybar-repo && \
chmod +x ~/.config/waybar/*.py && \
killall waybar && nohup waybar > /dev/null 2>&1 &
```

---

## 📂 File Structure

```
~/.config/waybar/
├── config.jsonc       # Main structure defining module order (Centralized)
├── style.css          # Visual soul — contains #8E00FF hex codes and pill shapes
└── window_pill.py     # Helper script for active window title detection
```

---

## 🙌 Credits

Maintained by **Douglas** 🚀
