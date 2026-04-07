# hyprlock-omarchy

Minimal, clean [hyprlock](https://github.com/hyprwm/hyprlock/) configuration extracted from my personal [Omarchy](https://github.com/basecamp/omarchy) setup.

This repo is intentionally small and self-contained. It only includes what is required to reproduce the lock screen, without pulling in a full dotfiles setup.

## Contents

- `hypr/hyprlock.conf` — main configuration
- `hypr/bindings.conf` — lock screen bindings configuration
- `scripts/hyprlock-bar-right` — wrapper script that outputs the artist playing and battery status
- `scripts/hyprlock-battery-indicator` — script that outputs the battery status
- `scripts/hyprlock-system-info` — script that outputs a bunch of system infos in a single line
- `scripts/waybar-now-playing` — script that outputs the currently playing artist (notice the naming pattern, you can also use this in your waybar)

## Preview

![Preview](preview.png)

## Requirements

- `hyprlock`
- `jq` (required by `scripts/hyprlock-bar-right`)
- `playerctl` (required by `scripts/waybar-now-playing`)
- A media player exposing MPRIS controls for `playerctl` (the current scripts target `jellyfin-tui`)
- A Nerd Font such as `JetBrainsMono Nerd Font` or change the font values in `hypr/hyprlock.conf`
- A battery sysfs path like `/sys/class/power_supply/BAT1` for `scripts/hyprlock-battery-incidator` (adapt if your battery is under a different path)

Make sure these are installed and available in your `$PATH`. If you are not using Omarchy, adjust the power bindings and theme source paths before applying the config.

## Installation

1. Clone the repo
2. Copy the configs you want
3. Copy the scripts you need
4. Double check your `$PATH` or use absolute paths for the scripts 
