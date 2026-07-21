# jellywear

A Jellyfin client for Wear OS — browse and play your music, audiobooks,
series, movies, and playlists straight from your watch.

This repo hosts installable builds only. It's updated automatically
whenever a new release ships.

## Download

[![Latest release](https://img.shields.io/github/v/release/Phat-shot/jellywear-release?label=latest%20release)](https://github.com/Phat-shot/jellywear-release/releases/latest)

Grab the newest APK from the **[latest release](https://github.com/Phat-shot/jellywear-release/releases/latest)**.

## Features

**Library, organized for a watch screen**
- Six home tiles: Music, Audio(books), Series, Movies, Favorites, and Playlists
- Music drills down properly (Artist → Albums → Songs), Series the same way (Series → Seasons → Episodes) — not just one flat list
- Favorites surfaces everything you've starred; Playlists lists yours with their tracks underneath
- Crown/rotary scrolling on every list

**Playback**
- Play/pause plus skip-forward/skip-back, with queue-aware controls
- Background playback via a real Android media session — audio keeps
  going (with system media controls) after you leave the app or the
  screen turns off
- **Long-press any folder, artist, album, series, or playlist to
  shuffle-play everything underneath it** — no need to open it first
- Video is cropped to fill the watch's width rather than shrinking to
  fit, so it doesn't play in a small letterboxed rectangle
- Optional cover art: off, shown in browse lists, or also as a dimmed
  background during playback

**Sign-in**
- **Quick Connect**: the watch shows a short code, you approve it from
  an already-signed-in phone or computer — no typing a password on a
  tiny screen
- Falls back to username/password (via Wear OS's voice/keyboard/
  handwriting input) if Quick Connect isn't enabled on your server
- If you don't type `http://`/`https://`, jellywear tries both

**Personalization**
- Theme: Dark, Light, or System
- Custom accent color and text color (a handful of presets, not a full
  color wheel — this is a watch, not a paint app)
- Language: follows your system language, or pin it to English, German,
  French, Spanish, or Arabic regardless of the system setting

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
