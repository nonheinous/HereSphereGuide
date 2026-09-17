# Autofocus and depth

Autofocus shifts the stereo image based on the depth of what you're looking at. It is off by default and works only on equirectangular and fisheye videos [2023-08], [2026-03].

| Task | Where |
| --- | --- |
| Turn autofocus on | *Advanced video settings*, toggle next to *Autofocus* [2023-08] |
| Hide depth numbers when paused | *Hide distance overlay* toggle, upper left of *Advanced video settings* [2024-12] |
| Improve accuracy | *User settings*, *Projection controls* group; higher costs performance [2022-06] |
| Stop constant shifting | Set *Autofocus distance override* to the subject's distance in cm [2026-02] |
| Limit bad depth guesses | Narrow min and max distance; add keyframes with the key icon for parts of a video [2023-11] |
| Reset autofocus values | Hover each and click the thumbstick or press A / X [2026-03] |

## Notes

- A closer distance override gives a stronger stereo effect [2026-02].
- Some double vision is normal in stereo 3D. *Force mono* looks sharper only because both eyes see the same image and depth is gone [2024-12].
- Very close objects block one camera's view, so autofocus can't measure them [2023-11].
- Depth readings are only accurate when the video is stitched correctly. See [Stereo alignment](stereo-alignment.md) [2024-05].
- Autofocus was disabled by default because it hurt performance on Quest 1 [2023-08].
