# HereSphere Web API

The Web API is a JSON interface that lets a server or website provide a browsable library, tags, scripts, subtitles, and HSP files to HereSphere. XBVR, stash-vr, and several studio sites implement it.

!!! note
    No public specification was posted in the source channel. This page lists behaviors the developer confirmed.

## For users

On a site that supports it, press the icon to the left of the URL bar that looks like a play button on four tiles, or add `/heresphere` to the end of the URL [2023-01], [2024-11].

## For developers

- Serve it at the `/heresphere` endpoint with the correct response header [2023-09].
- Items with `access` not set to 1 are treated as trailers, and their tags may not load [2025-04].
- Users need *Overwrite tags* enabled (cogwheel, bottom right) for updated tags to apply to videos already in their library [2025-04].
- Providing your own *Recently added* list controls display order [2025-01].
- If projection is detected wrong while testing, delete your server's entry from the Media Library to clear cached data, then reload [2025-01].
- The Quest 2 build once identified itself with the user-agent `HereSphere/0.8 Quest2`; current values are unconfirmed [2022-12].
