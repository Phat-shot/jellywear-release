# jellywear

A Jellyfin client for Wear OS — browse and play your music, audiobooks,
series, movies, and playlists straight from your watch, with background
playback, cover art, light/dark theming, and support for English, German,
French, Spanish, and Arabic.

This repo hosts installable builds only. It's updated automatically
whenever a new release ships.

## Download

[![Latest release](https://img.shields.io/github/v/release/Phat-shot/jellywear-release?label=latest%20release)](https://github.com/Phat-shot/jellywear-release/releases/latest)

Grab the newest APK from the **[latest release](https://github.com/Phat-shot/jellywear-release/releases/latest)**.

## Installing on your watch

Wear OS doesn't install APKs directly, so sideload it via one of:

- **ADB**: pair your watch for [debugging over Wi-Fi](https://developer.android.com/training/wearables/get-started/debugging), then
  ```bash
  adb install jellywear-vN.apk
  ```
- **A sideloading app on your phone** (e.g. "Wear Installer 2"), which pushes the APK to the watch over Bluetooth — no ADB needed.

## Requirements

- A Jellyfin server you can reach from your watch (local network or a reverse proxy)
- Wear OS 3 or newer

## Signing in

On first launch you'll be asked for your server address, then either:

- **Quick Connect** (if enabled on your server) — a short code is shown on the watch; approve it from an already-signed-in session on your phone or computer, no typing needed, or
- Username and password, entered via Wear OS's built-in voice/keyboard/handwriting input.
