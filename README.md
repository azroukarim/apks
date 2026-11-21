# Streamplayer v5 — build 5.3.43

APK de production pour Android TV / Android Phone.

## Fichiers

| Fichier | Architecture |
| --- | --- |
| `Streamplayer_v5.3.43_arm32.apk` | `armeabi-v7a` |
| `Streamplayer_v5.3.43_arm64.apk` | `arm64-v8a` |
| `Streamplayer_v5.3.43_x86_64.apk` | `x86_64` |

## Changes in 5.3.43

- MAG / Stalker Live: all channels category (`*`) is handled correctly.
- MAG / Stalker Live: uses the direct `cmd` URL when `create_link` returns an empty `stream=`.
- MAG audio: forces the libVLC AudioTrack output to stereo and selects VLC channel mixer mode `1` for Stalker streams, avoiding silence on stereo-only HDMI outputs.
- Android BACK returns to the previous screen instead of closing the app.
- Xtream and M3U playback behavior is unchanged.

## Installation

Install only the APK matching the device architecture:

```sh
adb install -r Streamplayer_v5.3.43_arm32.apk
```

## Vérification

```sh
sha256sum -c SHA256SUMS
```

Windows PowerShell:

```powershell
Get-FileHash .\Streamplayer_v5.3.43_arm32.apk -Algorithm SHA256
```
