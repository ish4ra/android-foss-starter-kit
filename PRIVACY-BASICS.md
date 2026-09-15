# Android privacy basics

Privacy improvements should not make the phone impossible to maintain.

## High-value changes

### Review app permissions

Pay special attention to:

- location;
- contacts;
- microphone;
- camera;
- notifications;
- accessibility service access;
- device admin;
- "install unknown apps" permission;
- VPN profiles.

If an app does not need a permission for its core job, deny it first and enable it later only if required.

### Keep the OS and browser current

A privacy-focused browser that is months behind Chromium/Firefox security fixes is not a good trade.

The same rule applies to custom ROMs: prefer officially supported, actively maintained builds over random unofficial images.

### Reduce background access

Android already provides useful controls for battery/background behavior, permissions and notifications. Use them before adding aggressive task killers or questionable "optimizer" apps.

### Use private DNS or a local DNS filter when useful

Options include:

- Android Private DNS with a trusted provider;
- AdGuard Home / Pi-hole on your own network;
- Rethink DNS + Firewall for device-level control.

DNS filtering does not replace browser content blocking or app permissions.

### Protect authentication backups

If you use Ente Auth, Aegis or another TOTP app, keep recovery codes/exports somewhere you can access if the phone is lost.

### Prefer strong screen security

Use a strong PIN/password and biometrics as convenience, not as a substitute for a strong device credential.

## Custom ROM privacy

LineageOS can reduce vendor bloat and give supported devices a clean Android base, but it is not automatically the best choice for every security model.

Consider:

- bootloader state;
- update cadence;
- verified boot behavior;
- device support quality;
- banking/DRM compatibility;
- whether proprietary Google services are required by your apps.

Use [LINEAGEOS.md](LINEAGEOS.md) as a starting point.

## FOSS ≠ private by definition

Open-source apps can still connect to external services, request broad permissions, contain optional telemetry or have security bugs. Evaluate the actual behavior of the app and project.

## Practical target

A good privacy-oriented Android setup is one you can keep patched, backed up and usable every day.