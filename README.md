# Freebee Player

The app that runs on a Freebee Ads mall screen. It plays the ad loop and games full screen, reports the box's health (CPU, memory, disk, temperature, network, uptime) to the ops dashboard, keeps a crash log, accepts restart, reboot and on-screen messages from the dashboard, and updates itself at night.

This repository only holds the installers. The source lives in a private repository.

## Download

Get the latest build for your box from the Releases page on the right, or from https://freebeeads.com/download, which also shows the checksum for each file.

| Box | File |
| --- | --- |
| Android TV box or tablet | `freebee-player-<version>.apk` |
| Windows mini PC | `Freebee-Player-Setup-<version>.exe` |
| Mac mini | `Freebee-Player-<version>.dmg` |

## Install and test

The full guide for a non-technical ops person is at https://freebeeads.com/docs/repo/player-install: install on each kind of box, pair it with its screen, run the camera walk-past test, simulate a power cut and a wifi cut, and send a test message and a restart from the dashboard.

Current builds are unsigned (Mac, Windows) or signed with a temporary key (Android), so the first start needs the one-time Open Anyway (Mac) or SmartScreen More info > Run anyway (Windows) step described in the guide.

## Checksums

Every release carries a `SHA256SUMS.txt`. Check a download with:

```
shasum -a 256 -c SHA256SUMS.txt
```
