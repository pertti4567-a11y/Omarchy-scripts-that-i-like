# Omarchy scripts that I like

A personal toolkit for making an **Omarchy + Hyprland** desktop more comfortable, flexible, and keyboard-driven. It brings together small utilities, input-device setup, and window-manager shortcuts for the everyday things I want my Wayland setup to do.

> **Platform:** Omarchy, Hyprland, and Wayland. Some input-related features use Linux `evdev`, `uinput`, or `keyd`.

## What this project is for

This repository is a home for the scripts and configuration I use to shape my Omarchy workflow. The goal is to keep useful desktop actions close at hand: control a mouse, manage a window, adjust a device, or move between monitors without breaking focus and reaching for a separate app.

The collection is personal and may depend on the machine's devices, permissions, installed packages, and Hyprland configuration. Review each script and setting before using it, and adapt the keybindings and device details to your setup.

## Toolkit highlights

- **Autoclicker** — trigger repeated mouse clicks for workflows where automated clicking is useful.
- **DPI switching** — change mouse sensitivity without digging through desktop settings.
- **Force-close shortcut** — quickly deal with a stuck or unresponsive window.
- **Hover-window volume** — control the volume of the window under the pointer, rather than needing to focus it first.
- **Replay clips** — keep a quick replay or clip workflow available from a hotkey.
- **Input setup** — configure the supporting `keyd` and `uinput` pieces used by input-related tools.
- **Hyprland bindings** — connect these actions to shortcuts that fit an Omarchy keyboard workflow.
- **Next-monitor focus** — includes the `Super+§` binding to focus the next monitor.

## Requirements and compatibility

The configuration is intended for an Omarchy desktop running Hyprland on Wayland. Depending on which parts you use, you may also need:

- Linux input-device support (`evdev` and/or `uinput`);
- `keyd` for the relevant keyboard remapping setup;
- permissions that allow the selected input utility to access its device or create a virtual input device;
- the applications or command-line tools used by the particular script; and
- a keyboard layout where the `§` key is available as expected.

Requirements can vary by script and machine. Check the script and its comments for its actual dependencies before enabling it. Input-device access and service configuration can affect the whole desktop, so avoid running commands or granting permissions you do not understand.

## Setup

1. Clone or download this repository.
2. Review the scripts and configuration before running or installing anything.
3. Install only the dependencies required by the features you want to use.
4. Configure `keyd`, `uinput`, and any device permissions required by your setup.
5. Add or adapt the Hyprland bindings in your Omarchy/Hyprland configuration.
6. Reload Hyprland and test each shortcut individually.

This is a personal toolkit rather than a universal installer: device names, package names, permissions, and configuration locations can differ between systems. Back up your existing configuration before making changes.

## Hyprland shortcut notes

The bindings are meant to make these utilities quick to reach and easy to customize. In particular, **`Super+§` focuses the next monitor**. If that key does not work on your keyboard, check how your layout and Hyprland identify it, then change the binding to a key that is convenient for your setup.

Before adding bindings, make sure the command they invoke is installed and that its path matches your machine. Avoid duplicate shortcuts that already have a different action in your Omarchy configuration.

## Safety and troubleshooting

- **A command does not run:** check that its dependency is installed and that the configured command or script path is correct.
- **An input feature cannot access a device:** inspect the relevant `keyd`/`uinput` setup and device permissions; do not make device files broadly accessible as a workaround.
- **A shortcut does nothing:** check for a conflicting binding, confirm the key name for your layout, and reload Hyprland after editing the configuration.
- **A feature behaves differently on another machine:** input devices and Wayland permissions vary, so review and adjust the setup rather than assuming every device uses the same name or settings.

## About

These are **my Omarchy things**: practical scripts and hotkeys for the desktop I use and the workflow I want. Feel free to adapt the ideas for your own setup, but check each feature against your system before enabling it.
