# Versions, install and updates

Pick the version that matches where the app will run. Each platform is a separate purchase; the one exception is that itch.io buyers can request a Meta store key [2024-11].

| Version | Runs on | Updates | Notes |
| --- | --- | --- | --- |
| Meta store (formerly App Lab) | Quest headset, standalone | Automatic | Release-candidate channel available on the store page [2026-01] |
| itch.io APK | Quest headset, sideloaded | Manual | Free demo available; email support from the purchase address for a Meta store key [2024-11] |
| Steam | Windows PC, streamed to headset | Through Steam | Needs SteamVR and a link cable, Air Link, Steam Link, or Virtual Desktop [2026-02] |
| Apple Vision Pro | AVP | App Store | Supports photos, which Quest and PC do not yet [2026-07] |

## Checking your version

Open *User guide* at the bottom of the left side panel, then *About* [2024-07].

## Switching to the release-candidate channel (Quest, Meta store)

Visit the HereSphere Meta store page, log in, scroll down to the version, and select the RC channel [2026-01].

## Updating a sideloaded APK (Quest)

Install the new APK over the old one. **Do not uninstall first**, because that erases saved data [2023-06].

1. Install SideQuest's *advanced* installer on your PC. The easy installer cannot install your own APKs.
2. Enable developer mode on the headset and connect it by USB-C.
3. Log into itch.io with the account you purchased with to download the new APK. If you didn't create an account, create one with the purchase email, or use the download link from your original purchase email [2023-06].
4. In SideQuest, click the down-arrow icon and select the new APK.
5. Or, from a command prompt in the APK's folder: `adb install -r HereSphere-vX.apk`. The `-r` flag keeps saved data [2022-07].

Sideloaded builds appear under *Unknown sources* in the Quest app library, reached through the filter icon on newer Quest OS versions [2023-08].

## Moving from demo to paid (Quest)

In the demo, open *User settings* and press *Save Backup*. In the paid version, press *Load Backup* [2025-11].

## Not supported

- Pico 4 Ultra (no progress yet) [2025-06].
- Android phones as a sideloading host [2022-08].
