# Changelog

Published TiltTrace releases. Packages are attached to each [GitHub release](../../releases) and mirrored at [arbhlabs.com/tilttrace/](https://arbhlabs.com/tilttrace/).

Published artifacts are immutable: a released version is never rebuilt or replaced.

## Windows 1.2.1 / Android 0.0.6 — 2026-09-09

- Windows adds one-click Rocket League official Stats API setup.
- Existing Rocket League Stats API user configuration is backed up before TiltTrace writes its local telemetry config.
- The Windows package is explicitly published as an unsigned Windows build with SHA-256 verification.
- Android 0.0.6 remains the current Android app release.

| File | SHA-256 |
|---|---|
| `TiltTrace-1.2.1-Setup.exe` | `e7c14b3585f6aa32dfcd4707f941dce960a46666c2c541e5c9923fb57f883922` |
| `TiltTrace-1.2.1-win-x64.zip` | `bf1d4993f810d3d749a6a5a11932425d58974f01ebbae85c2c76d678c7c98016` |
| `TiltTrace-Bridge-1.2.1.apk` | `e1650e71547b28688ed12e5b0519148b5864cfc0756602004025bf00b18397a9` |
| `TiltTrace-0.0.6.apk` | `d067e1db5ede981a4d1fc7c27049498ab4e5824362f4b123eda9929276cee022` |

## Windows 1.2.0 / Android 0.0.6 — 2026-09-09

- Android now supports an independent session with an optional standard Android controller; a PC is not required.
- Windows retains standalone controller, local-session, Bluetooth heart-rate, and optional authenticated Android bridge workflows.
- Hybrid pairing remains optional and tolerates either endpoint disconnecting or being unavailable.
- Windows release tooling no longer contains a signing-secret fallback.

| File | SHA-256 |
|---|---|
| `TiltTrace-1.2.0-Setup.exe` | `0420a6c2f19a7e727f8c0ccac8d4df4829b8793aa16f6b83df41ea01204e9af6` |
| `TiltTrace-1.2.0-win-x64.zip` | `8bb21081889a5cb3c01f827cb9394639a469fe90763fd545e9d93913dff43e71` |
| `TiltTrace-0.0.6.apk` | `d067e1db5ede981a4d1fc7c27049498ab4e5824362f4b123eda9929276cee022` |

## 0.0.4 — 2026-09-08

- Added dynamic on-screen pairing QR code for instant phone camera scanning.
- Auto-filling pairing code and PC host deep links (`tilttrace://bridge`).
- Smart clipboard detection and 1-tap code copy with bulletproof mobile HTTP fallback.
- Built-in local HTTP server for 1-tap browser APK download to phone.
- 1-click ADB USB companion installation and auto-launch directly from Windows desktop UI.
- Direct APK file export button for offline sideloading.
- Multi-network adapter prioritization: filters link-local (APIPA) and prioritizes active LAN with default gateway.
- Android 14+ Foreground Service conformance (`FOREGROUND_SERVICE_TYPE_DATA_SYNC`).
- Comprehensive provider broadcast extra parsing (`value`, `bpm`, `heartRate`, `hr`).
- Automatic bridge start when testing connection.
- Socket `ReuseAddress` support to prevent port collision on rapid restart.

| File | SHA-256 |
|---|---|
| `TiltTrace-0.0.4-Setup.exe` | `684882c108e41346ae41d22588f1c623f24e1eed3f90d8e7ca3cfa561528006e` |
| `TiltTrace-0.0.4-win-x64.zip` | `340e9534012d5ef73eaf691eb7b89c28a783579822d155147297b56a714792d4` |
| `TiltTrace-Bridge-0.0.4.apk` | `6502703ddaa4ca6e90e836a0eeace894ee5cbae331362346fe8f6ad3f489fdb9` |

## 0.0.3 — 2026-09-07

- Hardened UI-thread session finalization preventing crash risk on session end.
- Removed unused offline-admin code.
- Excluded internal test fixture from the shipped release package.

| File | SHA-256 |
|---|---|
| `TiltTrace-0.0.3-Setup.exe` | `40fad11aed5aeb599dfa0e74071bda80a47c6b410bff882233fc4493bf0899a1` |
| `TiltTrace-0.0.3-win-x64.zip` | `0b9b855aea3100c8ad649172116bd73a0264b093320d0f714eaede6d72ebf454` |
| `TiltTrace-Bridge-0.0.3.apk` | `4516125dd71c0417f2810b0f3640282d4270228b7c018cabd44f34f6210ce88f` |

## 0.0.2 — 2026-09-07

- Fixed provider HR broadcasts being queued behind the Android receive loop and never transmitted.
- Added automatic heartbeat/reconnection and discovery across all active Wi-Fi broadcast routes.
- Persisted pairing configuration across Android service restarts.
- Fixed valid HR being discarded after Android sequence resets or new Windows sessions.
- Added PC-address fallback, provider-event diagnostics and automatic Private-network firewall setup.

| File | SHA-256 |
|---|---|
| `TiltTrace-0.0.2-Setup.exe` | `6e028b626485286a82a91e95d93ef1c92456aa598de3fae3b7f341824a5d3fbe` |
| `TiltTrace-0.0.2-win-x64.zip` | `af08b38f8cc69dc37ffbd96dd75d75f0203f14e90de9d96386930f601b9549d1` |
| `TiltTrace-Bridge-0.0.2.apk` | `7e353d673131a373f69ae54a5a3e8753637cd2ecf0ef6baf585d385ae49f6282` |

## 0.0.1 — 2026-09-07

- Synchronized Rocket League, heart-rate and XInput capture on one monotonic timeline.
- Tilt Score v1.0, Clutch Score v1.0, EventResponse, RecoveryHalfLife, PressureCurve, InputEntropy and ChokeWindow analytics.
- Standard BLE heart-rate support and optional authenticated Xiaomi Smart Band 9 Android bridge.
- Local SQLite session recording, interrupted-session recovery, saved-session reopening and PNG result cards.
- Deterministic synthetic fixture pipeline and 16 passing Windows tests.

Artifacts:

| File | SHA-256 |
|---|---|
| `TiltTrace-0.0.1-Setup.exe` | `62dabce07ad5706e6d82e938efc5fd7b87760ccb9d8fd788d383a631d83c74cc` |
| `TiltTrace-0.0.1-win-x64.zip` | `b4eabcbfa83b0b640639bc1daaa55fd06b92527bd98c8060f176fff9cc7c62da` |
| `TiltTrace-Bridge-0.0.1.apk` | `a6e1c7b3d6eaf187acc49b0174af191a951bb5e50864c91af65c4e3841c68491` |
