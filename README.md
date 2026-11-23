# Streamplayer v5 — build 5.3.61

APK de production pour Android TV / Android Phone.

## Fichiers

| Fichier | Architecture |
| --- | --- |
| `Streamplayer_v5.3.61_arm32.apk` | `armeabi-v7a` |
| `Streamplayer_v5.3.61_arm64.apk` | `arm64-v8a` |
| `Streamplayer_v5.3.61_x86_64.apk` | `x86_64` |

## Liens de téléchargement (HTTP)

```
http://192.168.0.87:8099/Streamplayer_v5.3.61_arm32.apk
http://192.168.0.87:8099/Streamplayer_v5.3.61_arm64.apk
http://192.168.0.87:8099/Streamplayer_v5.3.61_x86_64.apk
```

## Changes in 5.3.61

- **ZOOM et sous-titres**: recadrage aligné en bas pour garder la bande de sous-titres visible (mpv dessine les sous-titres dans l'image vidéo).
- **Sous-titres séries**: la vérification par titre est ignorée pour les épisodes (OpenSubtitles renvoie souvent le titre de l'épisode), et la saison/l'épisode sont vérifiés quand disponibles.
- **Sous-titres films (5.3.59)**: filtrage par année, scoring de similarité du titre, rejet des candidats dont l'année ne correspond pas.
- **PLEIN** (5.3.58): remplit réellement l'écran.
- **Une touche** (5.3.58): affiche la barre d'infos (sans bouton œil).
- **Listes latérales** (5.3.57): défilement naturel.

## Installation

```sh
adb install -r Streamplayer_v5.3.61_arm32.apk
```

## Vérification

```sh
sha256sum -c SHA256SUMS
```
