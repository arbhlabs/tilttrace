# TiltTrace

**Local Rocket League performance forensics for Windows.**

TiltTrace synchronizes Rocket League events, heart rate and controller behavior on one monotonic match timeline. It generates deterministic Tilt Score and Clutch Score analytics, event-response windows, recovery metrics, a post-match timeline and shareable PNG result cards.

## Download

Release packages are attached to every [release](../../releases). The current Windows installer, portable archive and optional Android bridge are also available from **[arbhlabs.com/tilttrace/](https://arbhlabs.com/tilttrace/)**.

| | |
|---|---|
| Current Windows version | **1.2.1** |
| Current Android version | **0.0.6** |
| Requires | Windows 10/11 x64 |
| Windows signing | **Unsigned Windows build** |
| Installer size | 77,297,524 bytes |
| Installer SHA-256 | `e7c14b3585f6aa32dfcd4707f941dce960a46666c2c541e5c9923fb57f883922` |

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
Get-FileHash .\TiltTrace-1.2.1-Setup.exe -Algorithm SHA256
```

Expected SHA-256:

```text
e7c14b3585f6aa32dfcd4707f941dce960a46666c2c541e5c9923fb57f883922
```

Windows packages are currently unsigned and distributed with SHA-256 verification. Windows may show a security warning. The Android app and the optional Android bridge are release-signed by ARBH Labs.

## Issues and feedback

Bug reports are welcome in [Issues](../../issues). Include Windows version, TiltTrace version, input devices and the non-sensitive portion of the local diagnostic message.

---

Built by [ARBH Labs](https://arbhlabs.com/).
