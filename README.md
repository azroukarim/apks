# Streamplayer v5 — build 5.3.53

APK de production pour Android TV / Android Phone.

## Fichiers

| Fichier | Architecture |
| --- | --- |
| `Streamplayer_v5.3.53_arm32.apk` | `armeabi-v7a` |
| `Streamplayer_v5.3.53_arm64.apk` | `arm64-v8a` |
| `Streamplayer_v5.3.53_x86_64.apk` | `x86_64` |

## Liens de téléchargement (HTTP)

```
http://192.168.0.87:8099/Streamplayer_v5.3.53_arm32.apk
http://192.168.0.87:8099/Streamplayer_v5.3.53_arm64.apk
http://192.168.0.87:8099/Streamplayer_v5.3.53_x86_64.apk
```

## Changes in 5.3.53

- **Resume confirmation dialog**: when a movie or an episode has a saved position, a small window now asks whether to start from the beginning or continue from the last frame. No automatic jump any more.
- **Series seeking fixed**: LEFT / RIGHT always seek ±10 s in movies and episodes, even while an info-bar button is highlighted. DOWN cycles the info-bar buttons and UP walks back to the video.
- Completed items clear their saved position automatically; a position close to the end is still kept so the dialog can offer a restart.
- Keeps the 5.3.52 features: refresh scheduler, Nouveautés / Derniers lus bouquets, bouquet visibility editor, VLC full-screen fix and 4K/UHD playback settings.

## Installation

Install only the APK matching the device architecture:

```sh
adb install -r Streamplayer_v5.3.53_arm32.apk
```

## Vérification

```sh
sha256sum -c SHA256SUMS
```

Windows PowerShell:

```powershell
Get-FileHash .\Streamplayer_v5.3.53_arm32.apk -Algorithm SHA256
```
