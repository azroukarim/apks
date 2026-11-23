# Streamplayer v5 — build 5.3.67

APK de production pour Android TV / Google TV / Fire TV, téléphones et tablettes.

## Fichiers

| Fichier | Architecture |
| --- | --- |
| `Streamplayer_v5.3.67_arm32.apk` | `armeabi-v7a` (boîtiers TV 32 bits) |
| `Streamplayer_v5.3.67_arm64.apk` | `arm64-v8a` (téléphones/tablettes et TV 64 bits) |
| `Streamplayer_v5.3.67_x86_64.apk` | `x86_64` (émulateurs / TV x86) |

## Écran d'accueil

L'écran d'accueil **Streamplayer** (En direct, Films, Séries, Compte,
Changer la liste, Paramètres, Recharger, Quitter) est toujours la première
page de l'application, même lorsqu'aucun serveur XTREAM / MAG / M3U n'est
configuré. Les serveurs s'ajoutent depuis **Changer la liste**.

## Mise à jour automatique

`version.json` décrit la dernière version publiée. Au lancement, l'application
lit ce fichier sur GitHub. Si une version plus récente existe, une fenêtre
propose **Mettre à jour** ou **Plus tard**.

- **Mettre à jour** : télécharge l'APK correspondant à l'ABI de l'appareil,
  vérifie son SHA-256 puis ouvre l'installateur Android.
- **Plus tard** : ignore la proposition pour la session en cours.
- **Réglages → MISE À JOUR** : revérifie manuellement à tout moment.

Autorisez « Installer des applications inconnues » pour Streamplayer (et
désactivez l'Auto Blocker sur Samsung) lors de la première mise à jour.

## Liens de téléchargement (HTTP local)

```
http://192.168.0.87:8099/Streamplayer_v5.3.67_arm32.apk
http://192.168.0.87:8099/Streamplayer_v5.3.67_arm64.apk
http://192.168.0.87:8099/Streamplayer_v5.3.67_x86_64.apk
```

Liens GitHub (utilisés par la mise à jour automatique) :

```
https://raw.githubusercontent.com/azroukarim/apks/main/Streamplayer_v5.3.67_arm32.apk
https://raw.githubusercontent.com/azroukarim/apks/main/Streamplayer_v5.3.67_arm64.apk
https://raw.githubusercontent.com/azroukarim/apks/main/Streamplayer_v5.3.67_x86_64.apk
```

## Changements 5.3.67

- **Accueil toujours en premier** : l'application démarre sur l'écran
  d'accueil même sans aucun serveur ; « Changer la liste » ouvre la
  configuration XTREAM / MAG / M3U.
- **Réglages** : six tuiles en grille **3 colonnes × 2 lignes**.
- **Mise à jour intégrée** depuis GitHub (`Mettre à jour` / `Plus tard`).
- **Sous-titres ZOOM** placés sur l'image du film.

## Installation manuelle

```sh
adb install -r Streamplayer_v5.3.67_arm32.apk   # boîtier TV
adb install -r Streamplayer_v5.3.67_arm64.apk   # téléphone / tablette
```

## Vérification

```sh
sha256sum -c SHA256SUMS
```
