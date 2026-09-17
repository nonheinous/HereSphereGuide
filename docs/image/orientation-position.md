# Orientation, position and scale

## Recentering

- **Reset orientation** zeroes all orientation and origin settings and centers only the horizontal view, keeping you level with the real horizon [2022-05].
- **Recenter all** snaps the video center to your current head direction, including vertical. Use it when lying down [2022-07].
- **Recenter yaw** centers the horizontal rotation without resetting other values [2022-08].
- If recentering seems off, check the *Orientation* group for non-zero values. They're keyframed per video and add to your recenter [2022-05].

See [Controls](../getting-started/controls.md#recentering) for the default buttons.

## Motion

*Motion* simulates moving within the scene, like auto-zoom with head tracking. It is not true 6DOF [2023-04].

- Set *Motion distance* to the subject's distance, for example 50 cm, to make passthrough subjects feel fixed in place [2023-11].
- Grip + A recenters the motion position when the menu is hidden [2023-11].
- It warps the image somewhat, since the player can only stretch and shift the image [2026-08].

## Other settings

- **Keyframes** apply from their timestamp onward, including when paused or seeking [2023-11].
- **Lock the video to your head:** *User settings*, *Drag rotation acts as toggle* [2024-12].
- **Drag with your head instead of the controller:** *User settings*, *Drag rotation with head* [2022-07].
- **Horizontal flip:** PC only [2023-12].
- **Flat screens:** height and distance persist across videos; eye level can't be adjusted yet [2024-07].
- **Scale:** see [Stereo alignment](stereo-alignment.md#tips). If the camera was recorded at the wrong distance, getting both scale and position right is difficult; set scale first, then use Motion [2026-08].
