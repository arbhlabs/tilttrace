# TiltTrace

**Local Rocket League performance forensics for Windows.**

TiltTrace synchronizes Rocket League events, heart rate and controller behavior on one monotonic match timeline. It generates deterministic Tilt Score and Clutch Score analytics, event-response windows, recovery metrics, a post-match timeline and shareable PNG result cards.

## Download

Release packages are attached to every [release](../../releases). The current Windows installer, portable archive and optional Android bridge are also available from **[arbhlabs.com/tilttrace/](https://arbhlabs.com/tilttrace/)**.

| | |
|---|---|
| Current version | **0.0.2** |
| Requires | Windows 10/11 x64 |
| Installer size | 74,016,135 bytes |
| Installer SHA-256 | `6e028b626485286a82a91e95d93ef1c92456aa598de3fae3b7f341824a5d3fbe` |

## Inputs

- Rocket League official local Stats API.
- XInput-compatible controllers.
- Standard Bluetooth LE Heart Rate Service devices.
- Xiaomi Smart Band 9 through the optional TiltTrace Bridge Android companion and Notify for Xiaomi.

Gameplay, physiology and controller telemetry remain on the PC. The Android bridge transports current BPM over the local network using authenticated pairing and does not use a cloud service.

## About this repository

**TiltTrace is closed source.** This repository is not the source code. It hosts release binaries, checksums, the changelog and the public issue tracker, matching the distribution model used by other ARBH Labs applications.

TiltTrace is gaming-performance software, not a medical product. It does not provide diagnoses or clinical guidance.

## Verifying a download

```powershell
Get-FileHash .\TiltTrace-0.0.2-Setup.exe -Algorithm SHA256
```

Expected SHA-256:

```text
6e028b626485286a82a91e95d93ef1c92456aa598de3fae3b7f341824a5d3fbe
```

Windows packages are not Authenticode-signed in 0.0.2. The optional Android bridge is release-signed by ARBH Labs; its certificate SHA-256 fingerprint is `32679bae50998083d2e4df8aa39a5db80dad49101770bcb39262c4cce44fc8fc`.

## Issues and feedback

Bug reports are welcome in [Issues](../../issues). Include Windows version, TiltTrace version, input devices and the non-sensitive portion of the local diagnostic message.

---

Built by [ARBH Labs](https://arbhlabs.com/).
