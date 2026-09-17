# XBVR

XBVR is a free library manager that runs on your computer and serves videos, thumbnails, tags, scripts, and HSP files to HereSphere. It is the developer's recommended streaming setup for large libraries [2024-12].

For XBVR-side problems, the XBVR Discord is the better place to ask [2024-06].

## Setup

[2023-05]

1. Download XBVR for your computer from [github.com/xbapps/xbvr/releases](https://github.com/xbapps/xbvr/releases) and run it.
2. In a desktop browser, open `http://127.0.0.1:9999`.
3. In XBVR *Options*, add your video folders.
4. Under *Scrapers*, add the sites your videos came from.
5. After scraping, go to *Files*. Match any videos listed under *Unmatched* to the correct scene.
6. In *Options → Players*, note XBVR's IP address, usually starting with `192.`. On the HereSphere tab, enable the toggles for deleting files and syncing data if you want them.
7. In HereSphere's browser, enter `http://<XBVR IP>:9999/heresphere` and bookmark it once it loads [2026-05].

## Two-way sync

Syncing ratings, favorites, and tags needs both sides turned on [2022-11].

- **In XBVR:** *Options → Players → HereSphere*, enable the *allow … updates* toggles.
- **In HereSphere:** with XBVR loaded, click the cogwheel at the bottom right and enable *Overwrite tags*, *Overwrite favorite*, and *Overwrite rating*, then rescan the library [2022-09].

## Before migrating XBVR

HereSphere's saved settings are tied to XBVR's IP address and scene IDs. Before moving XBVR to a new computer, enable HSP and tag syncing to XBVR, or give the new machine the old IP address in your router [2025-03].

## Connection troubleshooting

[2023-05]

- Use the address of the computer running XBVR, not the headset's.
- Use a colon before the port (`:9999`), not a slash.
- Test the address from a phone's browser. If that fails, the problem is the PC, firewall, or router.
- Allow XBVR through Windows Firewall, then restart the PC and router.

## Other notes

- Subtitles and scripts must be matched to the scene in XBVR's UI. See [Audio and subtitles](../playing-videos/audio-subtitles-2d.md) and [Haptics](../haptics.md).
- Multipart scenes are delivered as encodings and can't be tagged individually [2023-02].
- XBVR watch history always appears in the Media Library; use a separate profile to avoid it [2025-08].
- If you also run ScriptPlayer, make sure XBVR and ScriptPlayer use different addresses or ports [2021-08].
