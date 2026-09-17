# Stash

Stash works with HereSphere through the stash-vr or stash-vr-companion add-ons, which serve a HereSphere Web API.

!!! note "Needs community review"
    Only 3 of 12 Stash questions in the source channel had developer answers. Corrections and setup steps from Stash users are especially welcome.

- HSP files must be served by stash-vr-companion; HereSphere can't load them from a local folder for Stash content [2025-09].
- `localhost` doesn't work in HereSphere's browser. On PC, type `127.0.0.1`. On Quest, use the Stash computer's LAN IP address, since localhost means the headset itself [2025-11].
- A playback error can mean the stream URL is unreachable, not just a codec problem [2025-10].
- Without an add-on, Stash's own web UI can load streams in HereSphere's browser [2024-01, community].
