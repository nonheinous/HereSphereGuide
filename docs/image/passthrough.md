# Passthrough and chroma key

Passthrough is available on Quest from version 0.10.0 and is set per video. See the [0.10.0 release notes](https://heresphere.itch.io/heresphere-vr-video-player-quest-2/devlog/635013/update-v0100-released) [2024-07].

## Turning it on for a video

1. In *Advanced video settings*, *Environment* group, set the background to *Pass through*.
2. Set *Mask* to match how the video was made:
    - **Alpha packed:** the mask is stored in the video's margins; look for solid-colored shapes there. Used by recent SLR videos [2024-09].
    - **Chroma key:** real green-screen footage [2024-07].
    - **HSP file:** some studios, like CzechAR, provide one beside the download. Put it in the same folder as the video [2024-01].
3. For alpha masks that don't line up, the cogwheel next to *Mask* has shift and scale settings [2023-11].

!!! warning
    Leave the global environment in *User settings* on *Color*. Setting it to *Pass through* forces passthrough on every video [2023-11].

## Chroma key settings

Open the cogwheel next to *Mask* [2025-09].

- **Key colors:** up to three, picked with the eyedropper. The eyedropper is much faster than entering values [2023-11].
- **Per key:** cutoff, soften, exponent, and spill mask control which pixels become transparent.
- **Despill color:** removes green halos and green tint on skin.
- **Light injection color:** adds color back to make despilled areas look natural.

Hold grip over any setting for its tooltip.

## Not supported

Masking part of a normal video to see your room through it [2024-02].
