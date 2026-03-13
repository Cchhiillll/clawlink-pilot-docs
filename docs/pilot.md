# Pilot Instructions (macOS client + macOS/Linux host)

Last updated: 2026-03-13

## 1) Download the macOS app
Direct download (recommended):
https://github.com/Cchhiillll/clawlink-pilot-docs/releases/download/v0.1.0-beta.3/ClawLinkMac-macos.zip

Fallback (if direct download has network issues):
https://github.com/Cchhiillll/clawlink-pilot-docs/releases/tag/v0.1.0-beta.3

Current public build:
- `v0.1.0-beta.3`

Download asset:
- `ClawLinkMac-macos.zip`


Install:
1) Unzip
2) Drag `ClawLinkMac.app` to Applications
3) Open it
4) If macOS blocks it, right-click `ClawLinkMac.app` → **Open**

## 2) Configure Base URL
Settings → Base URL:
- `https://clawlink.wypchill.work`

## 3) Register / Login
On the login screen choose **Register**:
- Email
- Password
- Invite code

**Invite code: please contact the pilot organizer.**

## 4) Host: install Bridge (macOS or Linux)

### macOS host
From the private repo on the host machine:
- Install Bridge service (launchd)
- Configure `~/.config/clawlink/bridge.env`

### Linux host (systemd)
From the private repo on the host machine:
- Install Bridge service (systemd)
- Configure `/etc/clawlink/bridge.env`

> If you need help installing Bridge on the host, contact the pilot organizer.

## 5) Pair host (QR → connect code)
On the host, generate a pairing QR.

Scan the QR on your phone to open the claim page and **copy the connect code**.

In the macOS app:
- Add Device → paste connect code

> Note: in-app QR scanner in macOS client is not complete yet. Current supported path is: phone scan QR → copy connect code → paste into Add Device.

## 6) Chat
- Select Device → Agent → Session
- Optional: switch Provider / Model in the chat header for the next message
- Send a message and confirm you get a reply
