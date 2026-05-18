# Changelog

## 0.1.0

Initial release.

- Packages the `bambu-studio-api` service from
  [`maziggy/orca-slicer-api`](https://github.com/maziggy/orca-slicer-api),
  branch `bambuddy/profile-resolver`.
- Bundles Bambu Studio AppImage `v02.06.00.51`.
- Runs on Ubuntu 22.04 with Node 22; amd64 only (Bambu Lab does not publish
  an ARM64 AppImage).
- Persists slicer profiles and uploaded presets under
  `addon_configs/<slug>_bambu_studio_api/data/`.
- Default host port `3001` to match the
  [Bambuddy wiki](https://wiki.bambuddy.cool/features/slicer-api/), editable
  via **Configuration → Network**.
- Watchdog and webui both hit `/health`.
