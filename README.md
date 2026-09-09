# Bluetooth Headsets

This is how I made bluetooth headset work with mpd.

## Packages required

```bash

pacman -Syu bluez bluez-utils pluseaudio-bluetooth mpd-mpris mpv-mpris mpd

```

## Enable mpd and mpris-proxy

I use `mpd` as my user:

```bash
systemctl --user enable --now mpd-mpris.service
systemctl --user enable --now mpris-proxy
systemctl --user enable --now mpd.socket
```


Now connect bluetooth device and enjoy play/pause, prev/next. 


