# Streamplayer v5 — build 5.3.59

APK de production pour Android TV / Android Phone.

## Fichiers

| Fichier | Architecture |
| --- | --- |
| `Streamplayer_v5.3.59_arm32.apk` | `armeabi-v7a` |
| `Streamplayer_v5.3.59_arm64.apk` | `arm64-v8a` |
| `Streamplayer_v5.3.59_x86_64.apk` | `x86_64` |

## Liens de téléchargement (HTTP)

```
http://192.168.0.87:8099/Streamplayer_v5.3.59_arm32.apk
http://192.168.0.87:8099/Streamplayer_v5.3.59_arm64.apk
http://192.168.0.87:8099/Streamplayer_v5.3.59_x86_64.apk
```

## Changes in 5.3.59

- **Sous-titres (OpenSubtitles / SubDL)**: sélection améliorée pour éviter les mauvais sous-titres. Filtrage par année et par épisode (séries), scoring de similarité du titre, rejet des candidats dont l'année ne correspond pas. On ne charge plus un sous-titre qui ne correspond pas au film.
- **PLEIN** (5.3.58): le vidéo remplit réellement l'écran.
- **Une touche** (5.3.58): affiche la barre d'infos (sans bouton œil).
- **Listes latérales** (5.3.57): défilement naturel.

## Installation

```sh
adb install -r Streamplayer_v5.3.59_arm32.apk
```

## Vérification

```sh
sha256sum -c SHA256SUMS
```
