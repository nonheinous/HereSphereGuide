# Audio, subtitles and 2D content

## Audio

- **Audio delay** for Bluetooth headphones is in *User settings* on current versions of both Quest and PC. If you don't see it, update the app [2024-10].
- **Multiscreen audio:** see [Playback features](playback-features.md#multiscreen).

## Subtitles

- Name the subtitle file exactly like the video, minus the video extension: `video.srt`, not `video.mp4.srt`. Copy and paste the name to avoid typos [2026-01].
- External SRT support arrived in release-candidate build 0.12.2 [2026-01].
- Over SMB, allow multiple simultaneous connections [2026-01].
- **Through XBVR,** subtitles must be matched to the scene in the XBVR UI; HereSphere can't see local files XBVR doesn't provide. If one stops working, clearing XBVR's cache often fixes it [2024-06]. XBVR controls the order of multiple files on a scene [2024-11].

## 2D videos

- Add `2D` to the filename to prevent VR detection. See [filename conventions](local-files.md#filename-conventions) [2024-09].
- Moving a 2D screen straight up or down isn't possible yet; rotating it is [2025-03].
- Flat screen height and distance persist from video to video [2024-07].

## Photos

Not supported on Quest or PC yet; planned for the next major update. The AVP version supports photos [2026-07].
