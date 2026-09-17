# Local files and folders

On Quest, copy videos to the headset's internal storage and open them from the HereSphere file explorer. Each folder you play from becomes a *media source* in the Media Library [2021-11].

- **Not supported:** USB storage plugged into the headset [2026-02], and reading a phone's storage [2024-06]. Stream over the network instead; see [Network sources](network-sources.md).
- **Selecting files:** the toggle beside each file selects it for adding to a playlist or deleting. The playlist and delete icons are at the top [2024-06].
- **Deleting is permanent.** Files are not sent to a recycle bin, and HereSphere never deletes folders [2022-08].
- **Subfolders:** add the root folder to a playlist to scan its subfolders [2022-08].
- **Fallback folders on Quest:** scripts go in `Interactive` at the root of storage; HSP files for DLNA content go in `HereSphere` at the root. Create the folder if it doesn't exist [2025-05], [2025-09].

## Filename conventions

Filename tags tell the player how to project a video before you touch any settings. The current list is at [heresphere.com/faq](https://heresphere.com/faq) [2024-10]. The last list posted in Discord [2022-09]:

| Add to filename | Result |
| --- | --- |
| `_180` | Equirectangular 180 |
| `_360` | Equirectangular 360 (limited adjustments; `_180` crops to the front half and enables autofocus) |
| `_F180` or `_180F` | Standard fisheye |
| `_MKX200`, `_MKX220`, `_RF52`, `_VRCA220`, `_FISHEYE190` | Custom fisheye lens profile |
| `_EAC360` or `_360EAC` | Equiangular cubemap |
| `_LR`, `_RL`, `_TB`, `_BT`, `_3DH`, `_3DV` | Stereo layout; without a projection tag, plays as a flat 3D screen |
| `_2D`, `-2D`, or a space before `2D` | Force 2D settings [2024-09] |

Spaces and hyphens work in place of underscores. With no tag, the player guesses from the video's aspect ratio, so 2D videos close to 2:1 can be misdetected as VR [2024-09].

There is no filename tag for rotation. To apply the same settings to many videos, save an HSP file for one, then copy and rename it to match the others [2023-11].
