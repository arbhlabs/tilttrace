# Changelog

Published TiltTrace releases. Packages are attached to each [GitHub release](../../releases) and mirrored at [arbhlabs.com/tilttrace/](https://arbhlabs.com/tilttrace/).

Published artifacts are immutable: a released version is never rebuilt or replaced.

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
