# Troubleshooting

Last updated: 2026-03-13

## Common issues

### 1) Can't register
- Make sure Base URL is `https://clawlink.wypchill.work`
- Invite code may be invalid/expired/revoked → contact organizer

### 2) Device stays offline
- Bridge service not running on host
- Host can't reach Cloudflare (network)

### 3) Can't claim device
- Code expired (codes are short-lived)
- Code already claimed

### 4) macOS app won't open after download
- Make sure you downloaded `ClawLinkMac-macos.zip` from the Releases page, not `Source code`
- Unzip first, then drag `ClawLinkMac.app` to Applications
- If macOS warns about the app, right-click `ClawLinkMac.app` and choose **Open**

## What to send for support
- Which step you are stuck on (1–6)
- Screenshot of the error
- Host bridge logs (if available)
  - macOS: `~/Library/Logs/ClawLink/bridge.log`
  - Linux: `sudo journalctl -u clawlink-bridge -n 200 --no-pager`
