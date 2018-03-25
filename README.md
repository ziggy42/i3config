# i3config
My personal configuration for i3.

## Hardware
`ThinkPad X1 Carbon`

## Distro
`Fedora 27`

## Dependencies
```bash
sudo dnf install i3 i3status dmenu i3lock xbacklight feh network-manager-applet lxappearance blueman
```

## Installation
```bash
link i3.config ~/.config/i3/config
link i3status.config ~/.config/i3status/config
```

## Fix brightness
Create the file `/etc/X11/xorg.conf` with the following content:
```
Section "Device"
    Identifier  "Card0"
    Driver      "intel"
    Option      "Backlight"  "intel_backlight"
EndSection
```

## TODO
- [x] Start Dropbox
- [x] Bluetooth indicator
- [ ] Desktop notifications
- [x] Screen brightness
- [ ] Colors
- [ ] i3block theme
- [ ] move to i3bar