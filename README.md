# Pi Configs

iOS-style desktop configuration for Raspberry Pi OS (Bullseye / LXDE).

## Contents

- `dock/` — Cairo Dock config (iOS-style, purple/blue frosted glass, 60px icons)
- `wallpaper/` — iOS-style deep blue/purple 4K gradient wallpaper
- `scripts/claude-widget` — Floating Claude AI launcher button (yad)
- `autostart/` — Autostart entries for Cairo Dock and Claude widget

## Setup

```bash
# Cairo Dock
cp dock/cairo-dock.conf ~/.config/cairo-dock/current_theme/
cp dock/_MainDock_-2.conf ~/.config/cairo-dock/current_theme/
cp -r dock/launchers ~/.config/cairo-dock/current_theme/

# Wallpaper
pcmanfm --set-wallpaper wallpaper/ios-wallpaper.png --wallpaper-mode=stretch

# Claude widget
cp scripts/claude-widget ~/.local/bin/
chmod +x ~/.local/bin/claude-widget

# Autostart
cp autostart/*.desktop ~/.config/autostart/
```
