# Stendhal

![img](https://github.com/Ruin0x11/Stendhal/blob/master/Other/sample.png)

A modified version of the [Stendhal](https://github.com/tatou-tatou/Themes/tree/master/Stendhal) theme by [tatou-tatou](https://github.com/tatou-tatou) for bspwm, without patched packages.

Various things might be broken, but it shouldn't matter too much if you don't use the mouse interaction a lot.

## Requirements
* `bspwm`
* `sxhkd`
* `lemonbar`
* `dunst`
* `dmenu2`
* `compton`
* `devmon`
* `amixer`
* `acpi`
* `xinput`
* `clock` (from sutils)

### Optional
* `scrot` (screenshot hotkey)
* `mpd` (music player)
* `plank` (dock)
* `udevil` (rootless mount/unmount list)
* `setxkbmap` (keyboard layout switching)
* `light` (MacBook screen brightness)
* `kbdlight` (MacBook keyboard lights)
* `feh` (for wallpaper)
* `offlineimap` (mail count)
* `mygtkmenu` (menu when clicking in top-left corner)

### Replacable
These are the default programs I set to launch, but they can easily be replaced in the sxhkdrc.
* `urxvt` (with xft font support)
* `emacs`
* `surf`
* `chromium`

## Installation
Install the required programs. The optional programs add various useful features.

Symlink everything in `Core` and `Scripts` to a folder on your path.

Install the included fonts.

Place the included `.xinitrc` in your home directory. Set the wallpaper with `feh` or similar within it.

Use `Tatou.Xresources` as your `.Xresources` for the terminal theme.

### Mail Notification
The mail notification depends on the `mail-sync` and `panel-mail` scripts. Setup `offlineimap` to sync your mail into a Maildir inside the `mail-sync` script, then indicate the directory within `panel-mail`. Up to two mailboxes can be shown by default. The command to run when clicking the notification can also be changed in `panel-mail`.
