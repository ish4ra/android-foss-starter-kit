# Android FOSS app picks

This is a starter shortlist, not a dump of every F-Droid app.

## App management

- **Obtainium** — install/update apps directly from upstream release sources such as GitHub, GitLab and supported repositories.
- **Droid-ify** — modern F-Droid repository client with background updates and multiple install methods.
- **Aurora Store** — open-source Play Store client useful when you still need apps distributed through Google Play.

## Browsers

### Helium

Fast Chromium/ungoogled-Chromium-oriented browser with privacy/performance goals. Interesting enthusiast pick, but treat project maturity and update cadence as part of your browser security decision.

### Cromite

Chromium-based browser with privacy, ad-blocking and hardening changes. Good choice for people who want Chromium compatibility with stronger defaults.

### IronFox

Firefox-family privacy-focused Android browser. Useful if you prefer Gecko and extension-style workflows.

Do not pick a browser only from benchmark results. Security update speed matters more than a small performance win.

## Authentication and passwords

- **Ente Auth** — encrypted multi-device TOTP authenticator with a strong cross-platform sync story.
- **Aegis** — excellent Android-focused authenticator with encrypted local vault/backups.
- **Bitwarden** — open-source password manager client with hosted and self-hosted options.
- **KeePassDX** — strong local-first KeePass-compatible password manager.

## Keyboard

- **HeliBoard** — privacy-friendly AOSP-style keyboard focused on local operation.
- **FlorisBoard** — flexible open-source keyboard with modern customization.

## Files and transfer

- **Material Files** — polished file manager.
- **LocalSend** — send files across Android, Windows, Linux, macOS and iOS on the local network.
- **Syncthing-compatible clients** — useful when you want continuous device-to-device folder sync rather than one-off transfer.

## Email and communication

- **Thunderbird / K-9 Mail** — mature open-source email client family.
- **Element** — Matrix client for federated messaging.
- **Molly** — hardened Signal-compatible client; evaluate whether its release/support model fits your threat model before replacing the official Signal client.

## Media

- **VLC** — general-purpose media playback.
- **mpv-android** — lightweight power-user media player.
- **AntennaPod** — excellent podcast client.
- **NewPipe** — open-source YouTube frontend/client.
- **Jellyfin** — official/open-source clients for your own Jellyfin server.
- **Streamyfin / Moonfin** — community Jellyfin clients worth testing if you run Jellyfin.

## Photos and gallery

- **Fossify Gallery** — simple local gallery.
- **Ente Photos** — end-to-end encrypted photo backup/service with open-source clients.
- **Immich** — excellent option if you self-host your own photo server.

## Maps and travel

- **Organic Maps** — privacy-focused offline navigation.
- **OsmAnd** — powerful OpenStreetMap-based offline navigation and mapping.

## Notes and productivity

- **Joplin** — Markdown notes with flexible synchronization.
- **Notesnook** — encrypted notes with open-source clients.
- **Markor** — local Markdown/text notes and to-dos.
- **Tasks.org** — capable open-source task manager with CalDAV/DAV integrations.

## Utilities

- **Breezy Weather** — highly configurable open-source weather client.
- **Fossify Calendar / Contacts / Phone / Messages** — simple replacements for common utility apps where they fit your device.
- **OpenCalc** — clean calculator option.

## Network and privacy tools

- **Rethink DNS + Firewall** — DNS/firewall controls with per-app visibility.
- **NetGuard** — no-root per-app network filtering using Android's VPN interface.
- **WireGuard** — standard VPN client when you control/use a WireGuard endpoint.
- **Tailscale** — not a pure fully self-hosted stack by default, but extremely practical for private remote access; Headscale is a self-hosted control-plane alternative for advanced users.

## What I would install first

For someone moving from a normal stock setup:

```text
Obtainium
Droid-ify
Ente Auth or Aegis
Bitwarden or KeePassDX
LocalSend
AntennaPod
Organic Maps
Breezy Weather
one browser you can keep updated reliably
```

Then replace other apps only when the FOSS option is actually good for your workflow.