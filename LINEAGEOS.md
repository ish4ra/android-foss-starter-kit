# LineageOS: practical starter guide

LineageOS is one of the best-known open-source Android distributions and is especially useful when you want a clean Android base or want to extend the useful life of supported hardware.

This page is deliberately conservative: **device-specific instructions from the official LineageOS wiki always override generic advice here.**

## 1. Check official support first

Before downloading anything:

1. Find your exact phone model and codename.
2. Confirm it is currently supported by LineageOS.
3. Open the installation page for that exact device.
4. Read the whole page once before touching the bootloader.

Do not assume that two phones with similar retail names use the same firmware, recovery or partition layout.

## 2. Understand the trade-offs

A custom ROM can improve longevity and remove vendor bloat, but it can also change behavior you rely on.

Possible trade-offs include:

- bootloader unlocking usually erases user data;
- banking, DRM or Play Integrity-dependent apps may fail or have reduced functionality;
- proprietary camera processing may be worse than stock;
- some vendor features may disappear;
- warranty/service implications vary by device and country;
- relocking a bootloader with an unsupported configuration can brick some devices.

Do not flash a ROM only because a screenshot looks cleaner.

## 3. Back up before unlocking

Assume the unlock step will erase the device.

Back up:

- photos/videos;
- authenticator recovery codes or exports;
- Signal/WhatsApp-style chat backups where relevant;
- password databases;
- contacts/calendar if not synced elsewhere;
- downloads/documents;
- app-specific exports;
- anything stored only inside an app's private data.

Two-factor authentication deserves special attention. Losing the phone and your only TOTP database at the same time is avoidable.

## 4. Use the correct platform tools

Typical installations use Android platform tools such as `adb` and `fastboot`, but the exact sequence differs by device.

Good habits:

- use a reliable USB cable;
- install current platform tools from a trusted source;
- confirm `adb devices` works before rebooting into bootloader mode;
- confirm `fastboot devices` works when the device is in the correct mode;
- never paste commands written for a different phone.

## 5. Decide what Google compatibility you need

LineageOS itself is not the same thing as "stock Android with Google removed". Decide what you actually need before installation.

Common approaches are:

### LineageOS without Google apps

Good if most of your apps work without Google Play Services and you prefer a cleaner base.

### LineageOS + a compatible Google apps package

Useful if you need Play Store/Play Services compatibility. Follow the **current device/version-specific LineageOS instructions** for timing and compatibility; installing the wrong package or installing it at the wrong stage can cause problems.

### microG-oriented setups

microG can provide open-source replacements for some Google Play Services behavior, but support depends on the ROM/build approach. Do not assume a normal LineageOS installation automatically provides every microG requirement.

## 6. First boot checklist

After a successful install:

- finish basic setup;
- connect to Wi-Fi/mobile data;
- install pending LineageOS updates;
- verify calls/SMS/mobile data;
- test Wi-Fi/Bluetooth/GPS/NFC if your device has them;
- test camera/video recording;
- test fingerprint/biometrics;
- test your most important banking/authentication apps before fully migrating.

## 7. Build the FOSS layer

A clean LineageOS install pairs well with:

- **Obtainium** — upstream app updates;
- **Droid-ify** — F-Droid repositories;
- **Ente Auth or Aegis** — TOTP authentication;
- **Bitwarden / KeePassDX** — password management;
- **LocalSend** — local file transfer;
- **Organic Maps / OsmAnd** — navigation;
- **AntennaPod** — podcasts;
- **Fossify apps** — simple replacements for common utilities.

See [APP-PICKS.md](APP-PICKS.md).

## 8. Updates and major upgrades

Normal OTA updates are one of the advantages of a properly supported LineageOS device. Major-version upgrades can be different.

Before a major upgrade:

1. read the upgrade instructions for your device;
2. back up important data;
3. check whether recovery/firmware requirements changed;
4. check Google apps compatibility if you installed a package;
5. do not improvise around failed steps.

## 9. What not to do

- Do not flash builds from random file-hosting links because a video tutorial says so.
- Do not mix recovery/images from similar but different models.
- Do not skip the firmware version requirement on the official wiki.
- Do not relock the bootloader unless the device/ROM documentation explicitly supports it.
- Do not start without a backup and recovery plan.

## When LineageOS is a great choice

LineageOS is especially compelling when:

- your device is officially supported;
- vendor software is bloated or no longer updated;
- you want a near-AOSP experience;
- you are comfortable troubleshooting Android/ADB/Fastboot;
- the apps you depend on work with your chosen configuration.

If your stock ROM works perfectly and you depend heavily on proprietary banking/camera/vendor features, staying stock and using FOSS apps can be the better choice.