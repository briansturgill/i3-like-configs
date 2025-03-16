# Simplar i3-like app configurations for Windows, MacOS, FreeBSD, and Linux

## Where to get i3-like programs for your platforms

* Linux and FreeBSD, i3 under X... comes with distribution.
* Linux and FreeBSD, sway under Wayland... comes with distribution.
* Windows: `winget install GlazeWM`
* MacOS: `brew install aerospace` (requires MacOS Ventura or newer)
		- AeroSpace is still in beta.

## To use

I've made equivalent configuration files for i3, sway, GlazeWM and aerospace.

* For i3 on Linux and FreeBSD, copy `i3_config` to `~/.config/i3/config`.
* For sway on Linux and FreeBSD, copy `sway_config` to `~/.config/sway/config`.
* For GlazeWM on Windows, copy `windows_config.yaml` to `~/.glzr/glazewm/config.yaml`.
* For AeroSpace on MacOS, copy `mac_.aerospace.toml` to `~/.aerospace.toml`.

Generally only features available on all platforms are in the files.
This means that i3 stacking and tabbing are not supported.

## General

To exit Glaze use:`alt+shift+e`

To reload the config file use: `alt+shift+c`.

To open a terminal window, use: `alt+enter`.
Under Windows: bash is used, but `alt+shift+enter` is `pwsh` and `ctrl+alt+shift+enter` is `cmd`.

### Exceptions:

* Window "minimize" (`alt+m`) is supported only on Windows because the dock is available to unminimize.

* Linux/Freebsd supports dmenu for app launching with `alt+d`. Windows and MacOS have equivalent functionality natively.

### Direction Keys

In the below descriptons, <DirectionKey> is one of the `vi` keys:
	`'h'`, `'j'`, `'k'`, `'l'`
or arrow keys:
	`'left'`, `'down'`, `'up'`, `'right'`

## Windows (GUI object)

To change the window being focused, use `alt+<DirectionKey>`.

To move the window being focused, use `alt+shift+<DirectionKey>`.

To resize windows, use key `alt+r` (enters resize mode), then use `<DirectionKey>s` to obtain the desired size.
Use `esc` or `enter` to end resize mode.

To cycle between floating/tiling/fullscreen windows, `alt+space`.

To toggle a window between tiling and floating `alt+shift+space`.

To toggle a window between tiling and fullscreen `alt+f`.

To set a window to tiling `alt+t`.

To set tiling direction for new windows: horiZontal `alt+z`, Vertical, `alt+v`.

To close the focused window use:`alt+shift+q`

## Workspaces

There are ten, numbered 1-10, and are focused by keys `alt+1 .. alt+0`.

Move a window to a workspace using keys `alt+shift+1 .. alt+shift+0`.

To toggle between the current workspace and the previously used one, use key `alt+w`.

To focus the prev/next workspace, use `ctrl+alt+<DirectionKey>`.

## Displays

To move the current workspace to another display, use `ctrl+alt+shift+<DirectionKey>`.

