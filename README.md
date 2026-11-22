# Streamplayer v5 — build 5.3.50

APK de production pour Android TV / Android Phone.

## Fichiers

| Fichier | Architecture |
| --- | --- |
| `Streamplayer_v5.3.50_arm32.apk` | `armeabi-v7a` |
| `Streamplayer_v5.3.50_arm64.apk` | `arm64-v8a` |
| `Streamplayer_v5.3.50_x86_64.apk` | `x86_64` |

## Liens de téléchargement (HTTP)

```
http://192.168.0.87:8099/Streamplayer_v5.3.50_arm32.apk
http://192.168.0.87:8099/Streamplayer_v5.3.50_arm64.apk
http://192.168.0.87:8099/Streamplayer_v5.3.50_x86_64.apk
```

## Changes in 5.3.50

- **VLC full-screen playback fixed**: removed the invalid libVLC option `--audio-device=stereo`. This option made libVLC refuse to start (`can't create LibVLC instance`), so every full-screen VLC stream stayed on LOADING while mini-TV (MPV) worked. The MAG/Stalker stereo downmix is kept via `--aout=audiotrack`, `--stereo-mode=1` and `--no-spdif`.
- **4K / UHD playback**: MPV uses `hwdec=auto` (instead of `auto-safe`) so the Amlogic box really uses MediaCodec for 4K/10-bit HEVC instead of slow software decoding.
- **VLC 4K**: explicit hardware decoding (`HwAcc.full`) plus network/live caching and late-frame dropping.
- **ExoPlayer**: the player settings screen warns that ExoPlayer cannot decode 4K/HEVC on this box (audio only) and recommends Internal (MPV).
- **Bouquets editor**: per-playlist visibility for Live TV / Movies / Series (Xtream and MAG), opened from the playlist actions dialog.
- **Server switching fix**: `showDialog` no longer crashes in French/Spanish (global localization delegates added).
- **Add Playlist**: moving the remote cursor onto M3U / Xtream / MAG switches the form immediately; OK and touch still work.
- **Text fields**: explicit focus nodes and `TextInputAction.next` let the remote move between fields with UP/DOWN (after closing the on-screen keyboard) or the keyboard's Next/Enter key.
- **Header focus indicator**: a thin accent underline appears under the focused header button without changing its width.
- MAG / Stalker Live, the stereo audio fix, Android BACK navigation and Xtream/M3U playback behavior are unchanged.

## Installation

Install only the APK matching the device architecture:

```sh
adb install -r Streamplayer_v5.3.50_arm32.apk
```

## Vérification

```sh
sha256sum -c SHA256SUMS
```

Windows PowerShell:

```powershell
Get-FileHash .\Streamplayer_v5.3.50_arm32.apk -Algorithm SHA256
```
