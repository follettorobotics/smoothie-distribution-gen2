# smoothie-distribution-gen2

OTA distribution channel for the **gen2** smoothie kiosk program.

- `latest.json` — manifest polled by gen2 kiosks (in-app updater).
- `changelog.json` + `index.html` — public changelog page (GitHub Pages).
- Releases carry the signed APK as `app-release.apk`.

Published automatically by `release-gen2.yml` in the app repo on annotated
`gen2-vX.Y.Z` tags. versionCode band: **+2,000,000** (rev0 = base band,
ICE20 = +1,000,000). This channel serves gen2 machines only — rev0 and
ICE20 fleets poll their own repos and never see these releases.
