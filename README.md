# ClawLink Pilot (Beta)

Last updated: 2026-03-13

This repo contains **pilot user documentation and download links** for ClawLink.

- Backend base URL: https://clawlink.wypchill.work
- macOS download: see **Downloads** below

> No code, no secrets are stored in this repo.

## Downloads
- **Direct download (recommended):** https://github.com/Cchhiillll/clawlink-pilot-docs/releases/download/v0.1.0-beta.3/ClawLinkMac-macos.zip
- Latest public macOS build: `v0.1.0-beta.3`
- Download asset name: `ClawLinkMac-macos.zip`
- Public releases page (fallback): https://github.com/Cchhiillll/clawlink-pilot-docs/releases


### Version Downloads
- `v0.1.0-beta.3` (release page): https://github.com/Cchhiillll/clawlink-pilot-docs/releases/tag/v0.1.0-beta.3
- `v0.1.0-beta.2` (release page): https://github.com/Cchhiillll/clawlink-pilot-docs/releases/tag/v0.1.0-beta.2
- `v0.1.0-beta.1` (release page): https://github.com/Cchhiillll/clawlink-pilot-docs/releases/tag/v0.1.0-beta.1

## Getting started (Pilot)
Follow: `docs/pilot.md`

Core flow (macOS app): **Device → Agent → Session → Chat**

## Current capability scope (important)
- ✅ Supported now:
  - Download macOS app, register/login, add device by connect code, and chat.
  - Host-side pairing QR generation + claim page flow.
- ⚠️ Not fully supported yet:
  - macOS client direct QR scanning/recognition for pairing (in-app scanner flow is not complete yet).

## Troubleshooting
See: `docs/troubleshooting.md`

## Release maintenance rule
For every new public release, update these docs in the same PR:
- `README.md` (latest version + direct download link + capability scope)
- `docs/pilot.md` (step changes + known limitations)
- `docs/troubleshooting.md` (new known issues/workarounds)
