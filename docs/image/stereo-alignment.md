# Stereo alignment and stitching

These settings correct videos where the two camera images don't line up. Some studios stitch well enough that you rarely need them [2023-04].

Make adjustments with autofocus on and the video paused. Depth readings then appear over the image, and those readings are your reference for what's correct [2023-10]. See [Autofocus and depth](autofocus.md) to turn them on.

## Quick fix (most videos)

[2022-06]

1. Enable autofocus, pause the video, and hide the menu.
2. Hold grip and move the thumbstick up or down until depth readings match what you'd expect in real life. This adjusts stitch shift X.
3. If scale still feels off, adjust *Camera stereo alignment right*.

## Full workflow

The developer's own process [2021-07]. Some of these key bindings are only bound to the keyboard by default; bind them to your controller first.

1. Look straight ahead. Adjust stitch (sensor) shift X, moving the left and right images in opposite directions, until distances look correct.
2. Still looking ahead, sweep stitch shift Y back and forth until the depth text looks sharpest.
3. Look at the top or bottom edge. Adjust stitch scale Y until the text is sharp there too.
4. Look at the left and right edges. Adjust stitch scale X until those distances are correct.
5. Adjust stereo alignment roll until the text is sharp at both side edges.

If roll can't fix both sides, adjust pitch while re-correcting shift Y. If depth at the top and bottom is off, adjust yaw while re-correcting shift X. If far objects line up better than close ones, try the camera stereo alignment up and forward settings.

Disable *Motion* and reset its position before starting, to reduce variables [2021-07].

## Tips

- **Opposite vs. same direction:** the two-arrows icon at the top of the stitch settings applies changes to each eye in opposite directions [2023-04]. A curved ceiling is corrected in the same direction, since both eyes are distorted the same way [2024-01].
- **Target distance:** adjust while looking at objects 100–200 cm away. At 200 cm, ±50 cm of error is fine; at 50 cm, ±5 cm matters. Use known objects, like a bed or couch, to judge distance [2023-02].
- **Camera stereo alignment right** is the camera IPD in cm. Most cameras are 6.4–6.5; some studios range from 6.0 to 8.0 [2021-07], [2022-03]. Increasing it makes things look bigger. It has more effect on close objects [2024-11], [2026-01].
- **Stereo alignment yaw** rotates each eye by half the value; stitch shift X shifts the image and changes depth at the top and bottom more [2022-08].
- **"Stereo" means stereoscopic 3D,** not stereo audio [2024-10].
- **Anaglyph view** is PC-only, and the depth text works better anyway [2023-10].

## Not fixable

- "Liquid" motion from out-of-sync left and right frames, which needs video editing [2022-02].
- Missing depth behind objects, since the stereo image is static [2025-11].
