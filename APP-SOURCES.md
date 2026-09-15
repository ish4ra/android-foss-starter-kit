# Android app sources

Where you install an app from matters almost as much as which app you choose.

## Recommended order

### 1. Official developer release

Best when the developer publishes signed APKs directly from an official project page or repository.

### 2. Obtainium

Obtainium tracks upstream releases and can update apps from supported sources such as GitHub, GitLab, Codeberg/Forgejo, F-Droid repositories and direct release pages.

Why it is useful:

- keeps you close to upstream;
- avoids manually checking dozens of GitHub release pages;
- works well for FOSS apps not available in Play Store;
- can notify you when new versions appear.

Caveat: some sources are tracked through scraping, so a website change can temporarily break update detection.

### 3. F-Droid repositories through Droid-ify

Droid-ify is a modern client for F-Droid-style repositories.

Good for:

- browsing FOSS software;
- adding trusted third-party repositories;
- background updates;
- offline browsing after repository metadata sync.

Remember that an F-Droid build and an upstream developer build can have different signatures. Do not casually switch between differently signed builds of the same package.

### 4. Aurora Store / Play Store when needed

Not every useful app is FOSS, and some essential banking, transport, government or work apps may only be distributed through Google Play.

A practical FOSS-first phone can still use proprietary apps when there is no sensible replacement.

## Avoid

- random APK mirror/mod sites for apps that have an official source;
- Telegram/Drive links with no verifiable upstream;
- "premium unlocked" APKs;
- old APKs copied between phones without checking signatures/version;
- installing certificate/profile/root modules you do not understand.

## Verify the project

Before installing a lesser-known app:

1. find the official website/repository;
2. check whether releases are current;
3. check the license/source;
4. confirm the package name where possible;
5. review permissions after installation;
6. keep it updated.

## A simple setup

For many users, this combination is enough:

```text
Play Store (apps that require it)
+ Obtainium (direct upstream FOSS releases)
+ Droid-ify (F-Droid ecosystem)
```

There is no prize for removing a store if doing so makes your phone harder to update securely.