<div align="center">

# Android FOSS Starter Kit

**A practical starter kit for building a cleaner Android setup with open-source apps, privacy-friendly tools, alternative app sources, and optional custom ROMs.**

**LineageOS is a first-class part of this guide — not a footnote.**

</div>

---

## What this repo is for

You do **not** need to remove every Google app or flash a custom ROM to benefit from FOSS Android software.

This guide supports three levels:

1. **Keep stock Android** and replace a few apps.
2. **Use FOSS-first app sources and utilities** while keeping Google Play where needed.
3. **Move to a custom ROM such as LineageOS** on a supported device when you understand the trade-offs.

The goal is a phone that is useful, maintainable and under more of your control — not ideological purity.

## Start here

| Goal | Guide |
|---|---|
| Pick FOSS apps | [APP-PICKS.md](APP-PICKS.md) |
| Install apps outside Play Store safely | [APP-SOURCES.md](APP-SOURCES.md) |
| Move to LineageOS | **[LINEAGEOS.md](LINEAGEOS.md)** |
| Basic privacy hardening | [PRIVACY-BASICS.md](PRIVACY-BASICS.md) |

## Recommended starter stack

| Need | Pick | Notes |
|---|---|---|
| App updates from upstream | **Obtainium** | Tracks releases from GitHub/GitLab/other sources |
| F-Droid client | **Droid-ify** | Modern F-Droid repository client |
| Browser | **Helium / Cromite / IronFox** | Different engines and maturity trade-offs |
| 2FA | **Ente Auth / Aegis** | Encrypted sync vs local-first Android focus |
| Passwords | **Bitwarden / KeePassDX** | Hosted/self-hosted vs local database |
| Files | **Material Files** | Clean open-source file manager |
| Nearby transfer | **LocalSend** | Cross-platform local file transfer |
| Keyboard | **HeliBoard / FlorisBoard** | FOSS keyboard options |
| Email | **Thunderbird / K-9 Mail** | Open-source mail client lineage |
| Podcasts | **AntennaPod** | Excellent open-source podcast app |
| Maps | **Organic Maps / OsmAnd** | Strong offline navigation options |
| Weather | **Breezy Weather** | Feature-rich open-source weather client |
| Gallery | **Fossify Gallery** | Simple local gallery |
| YouTube frontend | **NewPipe** | Lightweight open-source frontend/client |
| Network control | **Rethink DNS + Firewall / NetGuard** | Per-app network control without root |

## Why Obtainium matters

FOSS Android apps are often distributed directly by their developers rather than through one store. **Obtainium** can track upstream release pages and notify/install updates from supported sources, reducing the "random APK from a website" problem.

For F-Droid repositories, **Droid-ify** provides a cleaner client with background updates and multiple installation methods.

## LineageOS path

If your phone is officially supported, LineageOS can give old or vendor-abandoned hardware a clean Android base with long-lived community support.

Before flashing anything, understand these trade-offs:

- unlocking the bootloader normally wipes the phone;
- some banking/DRM/Play Integrity-dependent apps may behave differently;
- camera quality/features can differ from stock firmware;
- device-specific installation steps matter — never use another model's instructions;
- backups must happen **before** unlocking/flashing;
- OTA updates are straightforward once installed correctly, but major-version upgrades can require special steps.

Use the **official LineageOS device wiki/downloads** for your exact supported model. See [LINEAGEOS.md](LINEAGEOS.md).

## A realistic migration plan

Do not replace 25 apps in one evening.

```text
Week 1: Install Obtainium + one FOSS app you already need
Week 2: Replace browser, authenticator, file transfer and gallery
Week 3: Move more daily apps if the alternatives are genuinely better for you
Later: Consider LineageOS only if your device is supported and the ROM trade-offs make sense
```

## FOSS does not automatically mean secure

Open source improves transparency, but project maturity, update speed, browser engine security, signing, permissions and distribution source still matter.

For sensitive apps:

- download from the project's official source;
- verify you are using the correct upstream project;
- keep the app updated;
- avoid random mod APK sites;
- do not grant permissions an app does not need.

## Related guides

- **[open-source-alternatives](https://github.com/ish4ra/open-source-alternatives)** — broader desktop/web/self-hosted alternatives
- **[homelab-from-zero](https://github.com/ish4ra/homelab-from-zero)** — build a home server for self-hosted services
- **[selfhosted-picks](https://github.com/ish4ra/selfhosted-picks)** — apps worth hosting yourself

---

If this kit helps you build a better Android setup, a ⭐ helps other people discover it.