# Saved data, HSP files and backups

HereSphere stores its library in a binary file that can't be edited by hand, and its format changes between versions [2025-04]. The durable way to keep your work is HSP files.

## HSP files

An HSP file holds one video's image settings plus its tags and timestamps [2025-08].

| Task | How |
| --- | --- |
| Export one | *Advanced video settings*, save icon next to *Global settings*. The file lands beside the video, named to match [2025-09] |
| Export a folder | The folder's Media Library entry has a mass-export button [2025-04] |
| Create automatically | *User settings*, enable *Autoupdate HSP* and *Autocreate HSP* [2023-11] |
| Import | Place the HSP beside a same-named video. For a video you've already played, press the import button next to *Global settings* [2022-04] |

- **Moving or renaming videos** loses saved settings unless the HSP file moves with them [2024-07].
- **Over DLNA,** place HSP files in a `HereSphere` folder at the headset's storage root. **Over a web API,** the server must provide them [2025-09].
- **Over SMB,** the share user needs write permission for HSP files to be saved [2023-06].
- HSP files are binary and can only be read by HereSphere [2023-06].

## Backups

- **Quest:** *User settings*, *Save Backup* and *Load Backup*. Loading overwrites the whole library with the saved copy [2025-04].
- **PC:** saved data is at `%localappdata%/HereSphere/Saved/SaveGames`. Copy the folder to back up; delete it to reset to defaults [2024-06].

!!! tip
    Periodically back up, and turn on automatic HSP creation. Android prevents access to HereSphere's internal files on Quest, so HSP files and backups are your only copies [2023-04].

## Profiles

Entering a new profile name in *User settings* starts a separate library, which also works as a privacy password [2023-08].

- Profile names must match exactly when moving between headsets, because saved data is stored in a folder named after the profile [2023-10].
- Don't create a new profile on a headset that already has data you want to keep; the library won't copy over [2023-10].

## Web API data (XBVR, Stash)

Saved settings for web API content are keyed to the server's address and video URLs. Changing the server's IP address, or rebuilding a server with new IDs, orphans saved settings unless HSP sync to the server was on. See [XBVR](../integrations/xbvr.md#before-migrating-xbvr) [2025-03], [2025-04].
