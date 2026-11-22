# Streamplayer v5 — build 5.3.56

APK de production pour Android TV / Android Phone.

## Fichiers

| Fichier | Architecture |
| --- | --- |
| `Streamplayer_v5.3.56_arm32.apk` | `armeabi-v7a` |
| `Streamplayer_v5.3.56_arm64.apk` | `arm64-v8a` |
| `Streamplayer_v5.3.56_x86_64.apk` | `x86_64` |

## Liens de téléchargement (HTTP)

```
http://192.168.0.87:8099/Streamplayer_v5.3.56_arm32.apk
http://192.168.0.87:8099/Streamplayer_v5.3.56_arm64.apk
http://192.168.0.87:8099/Streamplayer_v5.3.56_x86_64.apk
```

## Changes in 5.3.56

- **Phone side lists**: the channel list and the bouquet list can now be scrolled by touch (swipe up/down). The parent video swipe detector no longer steals the gesture while a side list is open.
- **Web admin M3U**: added **Load now** / **Reload list** so an M3U playlist is downloaded directly on the TV/box from the browser, with a readable error when the provider is unreachable. A link such as `.../get.php?username=...&password=...` can be converted to an Xtream account with one tap.
- **Web admin Delete**: no longer relies on the native `confirm()` dialog (suppressed on some mobile browsers). Tap Delete twice to confirm; errors are shown in the page.
- **Episode playback (5.3.55)**: the info bar shows `position / duration` (e.g. `2:40 / 42:00`) and ±10 s seeking works even when the duration stream is missed, by polling the engine state once a second.

## Installation

Install only the APK matching the device architecture:

```sh
adb install -r Streamplayer_v5.3.56_arm32.apk
```

## Vérification

```sh
sha256sum -c SHA256SUMS
```

Windows PowerShell:

```powershell
Get-FileHash .\Streamplayer_v5.3.56_arm32.apk -Algorithm SHA256
```
