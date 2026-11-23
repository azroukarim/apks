# Streamplayer v5 — build 5.3.62

APK de production pour Android TV / Android Phone.

## Fichiers

| Fichier | Architecture |
| --- | --- |
| `Streamplayer_v5.3.62_arm32.apk` | `armeabi-v7a` |
| `Streamplayer_v5.3.62_arm64.apk` | `arm64-v8a` |
| `Streamplayer_v5.3.62_x86_64.apk` | `x86_64` |

## Liens de téléchargement (HTTP)

```
http://192.168.0.87:8099/Streamplayer_v5.3.62_arm32.apk
http://192.168.0.87:8099/Streamplayer_v5.3.62_arm64.apk
http://192.168.0.87:8099/Streamplayer_v5.3.62_x86_64.apk
```

## Changes in 5.3.62

- **Position des sous-titres**: remontés de 5 % environ pour ne plus coller au bord bas de l'écran.
  - MPV: `sub-pos=95`.
  - VLC: `--sub-margin=54` (marge positive = remontée dans libVLC).
  - ExoPlayer: marge basse 64 → 88 px.
- **Sous-titres séries (5.3.61)**: saison/épisode vérifiés quand disponibles.
- **Sous-titres films (5.3.59)**: filtrage par année et scoring du titre.
- **PLEIN** (5.3.58): remplit réellement l'écran.
- **Une touche** (5.3.58): affiche la barre d'infos (sans bouton œil).
- **Listes latérales** (5.3.57): défilement naturel.

## Installation

```sh
adb install -r Streamplayer_v5.3.62_arm32.apk
```

## Vérification

```sh
sha256sum -c SHA256SUMS
```
