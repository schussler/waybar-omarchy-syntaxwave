# 🟣 Custom Waybar Config for Hyprland (Omarchy-based)

A sleek, centralized, and performance-oriented Waybar configuration. This setup was built focusing on a clean developer workflow, featuring system monitoring and media controls with a vibrant deep purple aesthetic.

![Waybar Preview](https://img.shields.io/badge/Theme-Deep_Purple-8E00FF?style=for-the-badge)
![Platform](https://img.shields.io/badge/Platform-Arch_Linux-1793D1?style=for-the-badge&logo=arch-linux)
![WM](https://img.shields.io/badge/WM-Hyprland-33ccff?style=for-the-badge)

## ✨ Key Features

* **Centralized Layout:** All modules are grouped in a floating center pill for better focus on UltraWide and large displays.
* **Media Control (MPRIS):** Full Spotify/Media integration. 
    * *Left Click:* Play/Pause
    * *Right Click:* Next Track
    * *Scroll:* Previous/Next Track
* **Resource Monitoring:** Real-time **CPU** and **RAM** usage indicators to keep track of your development environment load.
* **Idle Inhibitor:** Quick toggle (Caffeine mode) to prevent screen sleep during long compilations or presentations.
* **Custom Aesthetics:** * Deep Purple accent (`#8E00FF`).
    * Clean "Pill" design with optimized padding and margins.
    * High-readability font (JetBrainsMono Nerd Font).

## 🛠️ Requirements

Ensure you have the following installed on your Arch system to make everything work perfectly:

```bash
sudo pacman -S waybar playerctl otf-font-awesome ttf-jetbrains-mono-nerd
