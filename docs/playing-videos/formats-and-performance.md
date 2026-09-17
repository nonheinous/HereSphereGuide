# Formats and performance

Prefer HEVC (H.265) downloads when a studio offers them. H.264 has poor compression above 4K, and hardware decoding for H.264 stops at 4K, so higher-resolution H.264 files stutter [2022-08], [2022-10].

## Frame rate

Keep the headset's refresh rate a multiple of the video's frame rate, which is usually 60 fps: 60, 120, 180, or 240 Hz. 120 Hz is the current sweet spot on standalone [2026-08].

60 Hz gives smoother playback, better performance, and better battery life if you can tolerate the flicker [2023-10].

## Resolution setting

*Resolution* in *Advanced video settings* is supersampling. Raise it until you can't see a difference; higher values cost framerate and battery. It matters most when sharpening is on [2024-11].

For 8K video on Quest, step it down in 0.05 increments until playback is smooth [2023-04].

## Codecs

- **AV1** should work on Quest 3. If a file freezes, try H.265 instead [2025-05].
- **Unsupported files** can't be skipped automatically yet [2024-11].
- **MKV rotation metadata** is ignored. For non-VR videos, use the screen orientation setting in *Advanced video settings* [2024-11].
- **PC:** see [PC version](../pc-version.md) for Media Foundation, DirectShow, and codec setup.
