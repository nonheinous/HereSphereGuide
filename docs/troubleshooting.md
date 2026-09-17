# Troubleshooting

When someone asks for help, the developer's first reply is usually a question: which version, which video source, or which file. Have those answers ready.

## Before asking for help, note

- **App version:** Quest standalone, PC, or AVP, and the version number from *User guide → About*.
- **Headset:** model and OS version.
- **Video source:** local, SMB, DLNA, XBVR, Stash, or a website.
- **Scope:** one video, some, or all. For one video, its resolution and codec.
- **What changed:** an app, headset OS, driver, or server update.

## General steps, in order

1. Restart the headset, the PC or server, and the router [2025-11].
2. Isolate the source: copy the file to the headset and play it locally, or try a website that uses the Web API. If that works, the problem is the network or server [2025-11].
3. For stutter or buffering over the network, use the router's 5 GHz band, and connect the PC to the router by Ethernet [2025-11].
4. Check for stale saved data. Delete the source's entry from the Media Library and reload it. On PC, reset `%localappdata%/HereSphere` after backing it up [2025-01], [2024-12].
5. If videos suddenly look wrong after an update, hover over each setting and reset it to default (thumbstick click or A / X) [2022-10].

## Common problems

| Problem | Likely cause and fix |
| --- | --- |
| No depth numbers when paused | Autofocus is off by default; enable it in *Advanced video settings* [2023-08] |
| Every video suddenly looks too big or warped | Changed default presets; reset FOV and origin, then re-save the first preset [2022-10] |
| Passthrough on for every video | Global environment set to *Pass through*; set it back to *Color* [2023-11] |
| Permission pop-up can't be clicked after update | Click the toggle, then press the Meta button to close; restart the headset if stuck [2023-09] |
| App missing from Quest library | Look under *Unknown sources* [2022-06] |
| Script, subtitle, or HSP not loading | Name mismatch; copy and paste the video name and check the extension [2026-01] |
| XBVR won't load | Wrong IP, slash instead of colon before the port, or firewall [2023-05] |
| Library loads slowly with XBVR | Thousands of videos in XBVR playlists; use saved searches [2022-12] |
| Screen drifts during playback | Controller thumbstick drift [2026-07] |
| "Finding position in room" persists | Possible headset sensor or camera hardware fault [2026-03] |
| Handy won't connect | See [Haptics](haptics.md#connecting-the-handy) |
