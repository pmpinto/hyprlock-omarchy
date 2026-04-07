# hyprlock-omarchy

Minimal, clean [hyprlock](https://github.com/hyprwm/hyprlock/) configuration extracted from my personal setup.

This repo is intentionally small and self-contained. It only includes what is required to reproduce the lock screen, without pulling in a full dotfiles setup.

## Contents

- `hypr/hyprlock.conf` — main configuration
- `hypr/bindings.conf` — lock screen bindings configuration
- `scripts/hyprlock-bar-right` — wrapper script that outputs the artist playing and battery status
- `scripts/hyprlock-battery-indicator` — script that outputs the battery status
- `scripts/hyprlock-system-info` — script that outputs a bunch of system infos in a single line
- `scripts/waybar-now-playing` — script that outputs the currently playing artist (notice the naming pattern, you can also use this in your waybar)

## Preview

IMAGE HERE

## Requirements

- `hyprlock`
- ...

Make sure these are installed and available in your `$PATH`.
Perhaps also make sure your `$PATH` in hyprland is consistent.

## Installation

1. Clone the repo
2. Copy the configs you want
3. Copy the scripts you need
4. Double check your `$PATH` or use absolute paths for the scripts 
