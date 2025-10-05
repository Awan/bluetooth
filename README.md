# Bluetooth Headsets

This is how I made bluetooth headset work with mpd.

## Packages required

```bash

pacman -Syu bluez bluez-utils pluseaudio-bluetooth mpd-mpris mpv-mpris mpd

```

## Enable mpd and mpris-proxy

I use `mpd` as my user:

```bash
systemctl enable --now mpd-mpris.service
systemctl enable --now mpris-proxy
```


Now connect bluetooth device and enjoy play/pause, prev/next. 


