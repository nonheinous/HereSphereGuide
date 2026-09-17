# PC version

The Steam version runs on a Windows PC and streams to the headset. It requires SteamVR; runtimes such as Virtual Desktop's VDXR are untested and would need a translation layer [2026-02]. An Nvidia GPU from the 10 series or newer gives the best hardware decoding [2023-02].

## Playback backends and codecs

The PC version offers two playback backends, selected in *User settings*.

| Backend | Codecs | Setup |
| --- | --- | --- |
| Media Foundation (default) | Windows Media Foundation | Install the free codecs from [codecguide.com](https://codecguide.com/media_foundation_codecs.htm); the old Microsoft Store HEVC link no longer works [2022-12] |
| DirectShow | LAV filters, typically through K-Lite | Install K-Lite, then switch backend [2023-11] |

- **DirectShow codec tweaks:** in the Codec Tweak Tool, set preferred decoders to *Use merit* or LAV Video for the formats you want, and make sure no DirectShow entries are disabled under codec and filter management [2025-05].
- **Windows N and KN editions** lack media codecs; install the Media Feature Pack [2022-07].
- **HEVC stopped working after a Windows repair:** reinstall graphics drivers [2022-07].

## Performance settings

- Set *MSAA* to 1 and *Resolution* to 2, or as high as holds your framerate [2022-12].
- For screen tearing over a link cable, lower HereSphere's resolution or the Oculus app's [2022-07].
- There is no refresh rate option in the PC version; set it in the headset or streaming software [2026-02].
- Air Link adds encoding load on top of decoding. Dropping to 60 Hz while the menu is open can be the PC falling short of 120 Hz [2022-12].

## PC-only features

- Anaglyph alignment view [2023-10] and horizontal flip [2023-12].
- YouTube and similar streams: put the `yt-dlp` executable in HereSphere's saved folder, then press the web stream icon left of the URL bar [2022-07].
- Mapped network drives stand in for SMB, which the PC version doesn't include [2022-05].

## If the app won't start or plays badly

1. Restart the PC. Launch Steam before HereSphere [2024-12].
2. Update, or roll back, the graphics driver. A 2026 driver update broke playback for one user [2026-03].
3. Reinstall SteamVR and the headset's desktop app [2023-11].
4. If videos on a local hard drive fail to play, switch the file explorer from thumbnail view to list view [2026-03].
5. Back up, then delete `%localappdata%/HereSphere` to reset saved data [2024-12].
