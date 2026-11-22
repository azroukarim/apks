# Streamplayer v5 — build 5.3.58

APK de production pour Android TV / Android Phone.

## Fichiers

| Fichier | Architecture |
| --- | --- |
| `Streamplayer_v5.3.58_arm32.apk` | `armeabi-v7a` |
| `Streamplayer_v5.3.58_arm64.apk` | `arm64-v8a` |
| `Streamplayer_v5.3.58_x86_64.apk` | `x86_64` |

## Liens de téléchargement (HTTP)

```
http://192.168.0.87:8099/Streamplayer_v5.3.58_arm32.apk
http://192.168.0.87:8099/Streamplayer_v5.3.58_arm64.apk
http://192.168.0.87:8099/Streamplayer_v5.3.58_x86_64.apk
```

## Changes in 5.3.58

- **PLEIN really fills the screen**: the MPV (default) engine now sizes its surface to the available space and stretches the picture with `BoxFit.fill`, so PLEIN covers the whole phone/TV screen instead of staying at the source resolution. VLC and ExoPlayer were aligned the same way.
- **One tap shows the info bar**: the permanent "eye" button was removed. A single tap anywhere on the phone screen now reveals the bar, even when the native video surface swallows touches (a transparent tap layer was added above the video).
- **Side lists (5.3.57)**: natural scrolling direction (swipe down advances), kinetic scrolling, highlighted row kept in view, counter follows scroll.

## Installation

```sh
adb install -r Streamplayer_v5.3.58_arm32.apk
```

## Vérification

```sh
sha256sum -c SHA256SUMS
```
