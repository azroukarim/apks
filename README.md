# Streamplayer v5 — build 5.3.52

APK de production pour Android TV / Android Phone.

## Fichiers

| Fichier | Architecture |
| --- | --- |
| `Streamplayer_v5.3.52_arm32.apk` | `armeabi-v7a` |
| `Streamplayer_v5.3.52_arm64.apk` | `arm64-v8a` |
| `Streamplayer_v5.3.52_x86_64.apk` | `x86_64` |

## Liens de téléchargement (HTTP)

```
http://192.168.0.87:8099/Streamplayer_v5.3.52_arm32.apk
http://192.168.0.87:8099/Streamplayer_v5.3.52_arm64.apk
http://192.168.0.87:8099/Streamplayer_v5.3.52_x86_64.apk
```

## Changes in 5.3.52

- **Refresh scheduler** in Settings: refresh channels, movies and series on every app start, every 24 h, every 48 h, every week, or never. A **Refresh now** button is also available.
- **Two smart bouquets** in Live TV, Movies and Series: **Nouveautés** (items added since the previous successful refresh) and **Derniers lus** (channels, movies or series already played). The first refresh creates the baseline so a whole catalogue is not reported as new.
- **Resume playback**: movies and episodes reopen at the saved position. The position is saved while playing and on exit; a completed item is cleared. Can be disabled from Settings.
- **Series history** records the parent series, so "Derniers lus" reopens the episode list instead of a single episode.
- All previous fixes are kept: bouquet visibility editor, VLC full-screen start fix, 4K/UHD playback settings, server-switch localizations, focus-based Add Playlist navigation, header focus underline, and movie/series next/previous controls.

## Installation

Install only the APK matching the device architecture:

```sh
adb install -r Streamplayer_v5.3.52_arm32.apk
```

## Vérification

```sh
sha256sum -c SHA256SUMS
```

Windows PowerShell:

```powershell
Get-FileHash .\Streamplayer_v5.3.52_arm32.apk -Algorithm SHA256
```
