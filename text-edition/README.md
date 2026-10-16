# Magium — Text Edition 0.2.2

An offline Android and browser edition of Cristian Mihailescu's original
interactive Magium Books 1–3, prepared with Flori Dumitrescu.

This edition uses **the existing game implemented by Thuiop and contributors**,
with its original parser, execution routines and story data. AI assistance was
used for the reading interface, offline integration, verification and Android
packaging. It does not replace the community's implementation or make their
work AI-created. The source archive documents the exact integration boundaries.

## Downloads

- [Android APK](Magium-Text-Edition-v0.2.2.apk?raw=true)
- [Self-contained browser HTML](Magium-Text-Edition-v0.2.2.html?raw=true)
- [Source, credits, tests and rebuild tools](Magium-Text-Source-v0.2.2.zip?raw=true)
- [SHA-256 checksums](SHA256SUMS.txt)

The browser file should be downloaded and opened in a browser that supports
local HTML applications. GitHub's file viewer is not the game player.

The Android APK requires Android 8.0 or later. Package: org.magium.textedition.
Version code 5, target SDK 36. Install over an existing Magium Text Edition
installation to preserve its local saves; do not uninstall first. This package
has its own identity, separate from Cristian's original Play application.

This is a development release for testing. It has not been submitted to or
approved by Google Play. Phone acceptance and further community testing continue.

## Included features

All 34 original chapters, choices, stats, achievements, 30 named save slots,
checkpoints, backup export/import, offline reading, adjustable text, themes and
typefaces. Back crosses text pages and Continue steps, stopping at genuine
choices. Next changes to Choose above when a choice is required.

All included books are unlocked during testing. There are no ads, purchases,
audio, story illustrations, analytics or private testing controls in this APK.
The original Magium emblem is included on the title screen and launcher icon.
Fresh reading settings default to 20px; existing preferences are preserved.

## Implementation and verification

Upstream port: https://github.com/thuiop/magium-dev

Pinned commit: 51f5aa9406c094e5133be2c7d69988296f86cfbc.

The vendored upstream files are retained unchanged. The integration has two
documented compatibility fixes: clearing a stale death flag on two Book 1
Chapter 3 scenes, and allowing the Book 3 consolation counter to advance beyond
the ordinary achievement guard. See ADAPTER.md in the source archive.

The public build passes 21 focused regressions and packaged offline-asset checks.
The prior reference comparison covered 2,159 scenes, 16,179 entry cases, 14,846
transitions and 16,148 valid snapshot roundtrips, with no unexpected mismatches
against the original routines plus those two corrections. These checks do not
prove every possible playthrough. jsdom checks are not physical Android tests.

The original signing key, text-edition save origin and save keys are retained.
No keys or passwords are included. The source includes the pinned native DEX
and scripts to reproduce APK/AAB packaging; it does not reconstruct that DEX.

## Credits and licences

- **Cristian Mihailescu:** story and original game.
- **Thuiop and contributors:** the existing port, parser, execution routines,
  story data, stat/state helpers, achievement metadata and community testing.
- **dragon_l:** acknowledgment for the earlier Android APK. This does not claim
  that our new Android wrapper is his code.
- **Radu:** release of the original source with Flori's permission.
- **Flori Dumitrescu:** preparation of this edition and provision of the original
  Magium emblem.
- **EJS 3.1.10, Matthew Eernisse and contributors:** offline templates, Apache 2.0.

Original source: https://github.com/raduprv/Magium

The original release identifies its story data as CC BY 4.0. Existing software
licence notices and EJS's full Apache notice are retained in the source, APK and
in-game Credits. The original emblem is not represented as being covered by the
software's MIT licence. See LICENSE, CREDITS.md, ATTRIBUTION.txt and vendor notices
in the source archive.
