# Network sources

On Quest, there are three ways to stream from a PC or NAS. The developer recommends XBVR if you have many videos, because it adds thumbnails, tags, and scripts [2024-12].

| Method | Best for | Scripts and HSP files | Notes |
| --- | --- | --- | --- |
| SMB file sharing | Simple folder access | Read from the same folder as the video | Setup varies by network and is the hardest to debug [2024-07] |
| DLNA media server | Existing media servers | Not shared; use fallback folders on the headset | Media files only [2025-05] |
| Web API ([XBVR](../integrations/xbvr.md), [stash-vr](../integrations/stash.md)) | Large libraries | Served by the app | Adds thumbnails, tags, and scripts |

## SMB file sharing (Quest)

!!! note "To do"
    The developer's one-page SMB setup image, pinned in Discord, is the standard answer to this question [2025-11]. It still needs transcribing here.

- Use the PC's network (NetBIOS) name, which is usually the computer name, instead of its IP address. That avoids breakage when the IP changes [2025-10].
- On Windows 11, if shares don't appear, open the Services app and set these to start automatically, then restart: *Function Discovery Provider Host*, *Function Discovery Resource Publication*, *SSDP Discovery*, *UPnP Device Host* [2022-03].
- For HSP files to save back to the share, the SMB user needs write permission [2023-06].
- Allow multiple simultaneous SMB connections, or subtitles and scripts may not load [2026-01].

**PC version:** there is no built-in SMB. Map the network drive in Windows instead [2022-05].

## Websites

Sites that support the HereSphere Web API load a full library view. Open the site in the in-app browser and press the icon to the left of the URL bar that looks like a play button on four tiles [2024-11].

For other sites, sign in and use the site's download link to stream [2024-04]. The browser does not support microphones [2025-11].

## Not supported

Streaming over a USB cable from a PC [2026-02]. Use the network, or run the [PC version](../pc-version.md) over Link or Air Link.
