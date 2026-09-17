# Projection, lens and FOV

Check FOV and lens type first. Some videos aren't truly 180° or weren't converted to equirectangular correctly [2021-07].

Leave the lens on linear for most studio videos, since studios usually linearize the image during editing. Lens profiles matter most for footage you shoot yourself and leave as fisheye [2022-05].

## Known settings by format

| Content | Settings |
| --- | --- |
| SLR MKX200 | Fisheye projection, MKX200 lens, 200 FOV; a small stitching fix may help [2023-08] |
| SLR 190° fisheye | Linear true lens, about 190 FOV [2025-01] |
| SLR Original Passthrough | Linear, 190 FOV [2025-09] |
| Video looks warped with no known profile | Try other lenses and FOVs; trial and error [2024-10] |
| Video recorded at 16:9 but shown distorted | Set aspect ratio to 2 [2021-06] |

## Notes

- **Export lens** matters only for equirectangular video, not fisheye [2025-01].
- **Switching projection partway through a video** (for compilations): click the key icon next to *Format*, then the plus icon to add a keyframe at the current time. Set the new projection; the player switches automatically at that point [2025-10].
- **Looking far left or right** shows little because most VR videos are only 180° [2026-08].
- **HEVC and fisheye** compress better than H.264 and equirectangular, so prefer them when offered [2022-08].
