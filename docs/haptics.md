# Haptics and synchronized peripherals

HereSphere drives script-synced devices in two ways: a direct connection for a few supported devices, or a timestamp server that sends playback position to a third-party app that controls the device.

| Device or app | How to connect | Notes |
| --- | --- | --- |
| The Handy | Direct: synchronized peripherals menu, enter connection key | Stroke range settings in the same menu [2023-05] |
| FL Launch, older Kiiroo Keon | Direct over Bluetooth | The only Bluetooth devices supported natively [2025-09] |
| Lovense and other Buttplug devices | Timestamp server → MultiFunPlayer, or ScriptPlayer + Intiface on PC | Not supported natively [2025-09] |
| OSR / SR6 | Timestamp server → MultiFunPlayer | MFP loads scripts itself [2023-11] |
| POVR scripts | Connect and Control, set up on POVR's site | Third-party service [2023-10] |
| SLR streaming scripts | Not supported; download scripts instead | Works only in DeoVR or SLR's app [2023-04] |

## Connecting the Handy

1. Click the icon above the seekbar that looks like a play button with radio waves [2024-05].
2. Enable *Synchronized peripherals* at the top.
3. Enter your Handy connection key. A status message confirms the connection.

If it won't connect [2024-07], [2024-11]:

- Confirm the Handy is in Wi-Fi mode (slow purple blink).
- Recheck the key: no spaces, exact capitalization.
- Power-cycle the Handy, then the router.
- Generate a new connection key on the Handy website.

## Using the timestamp server

1. In *User settings*, find the *Timestamp server* group.
2. Click the icon next to the IP address to fill it in automatically [2025-02].
3. Enter that IP address and port in MultiFunPlayer or ScriptPlayer. On PC, the address is `127.0.0.1` [2023-04].
4. Add your script folder in the third-party app. HereSphere sends only the video title, so script names must match it [2025-02].

In ScriptPlayer, use the DeoVR settings [2022-04].

## Script file matching

- Name the script exactly like the video, with a `.funscript` extension: `video.mp4` → `video.funscript`, not `video.mp4.funscript`. Copy and paste the name [2026-01]. CSV scripts also work [2022-08].
- **Local and SMB:** place the script in the same folder as the video [2022-06].
- **XBVR:** match the script to the scene in XBVR's UI [2023-07].
- **DLNA or websites:** put scripts in the `Interactive` folder at the headset's storage root, named to match the video title shown in the seekbar [2025-05], [2023-04].
- **Patterns:** files in `Interactive` whose names start with `Pattern` [2023-09].
