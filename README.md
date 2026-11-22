# Streamplayer v5 — build 5.3.54

APK de production pour Android TV / Android Phone.

## Fichiers

| Fichier | Architecture |
| --- | --- |
| `Streamplayer_v5.3.54_arm32.apk` | `armeabi-v7a` |
| `Streamplayer_v5.3.54_arm64.apk` | `arm64-v8a` |
| `Streamplayer_v5.3.54_x86_64.apk` | `x86_64` |

## Liens de téléchargement (HTTP)

```
http://192.168.0.87:8099/Streamplayer_v5.3.54_arm32.apk
http://192.168.0.87:8099/Streamplayer_v5.3.54_arm64.apk
http://192.168.0.87:8099/Streamplayer_v5.3.54_x86_64.apk
```

## Changes in 5.3.54

- **Phone controls fixed**: the info bar can now always be hidden and shown in Live TV, Movies and Series.
- Added an explicit **hide** button in the top bar and a permanent small **show** button when the controls are hidden. Tapping the info-bar background also hides it.
- Works around phones where touches on the native video view are not delivered to Flutter.
- Keeps the 5.3.53 features: resume confirmation dialog, reliable ±10 s seeking in series, refresh scheduler, Nouveautés / Derniers lus bouquets, bouquet visibility editor and 4K/UHD playback settings.

## Installation

Install only the APK matching the device architecture:

```sh
adb install -r Streamplayer_v5.3.54_arm32.apk
```

## Vérification

```sh
sha256sum -c SHA256SUMS
```

Windows PowerShell:

```powershell
Get-FileHash .\Streamplayer_v5.3.54_arm32.apk -Algorithm SHA256
```
