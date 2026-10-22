# Magium — Text Edition 0.2.15

Offline Android and browser edition of Cristian Mihailescu’s original interactive
Books 1–3: 34 chapters, 2,159 scenes and 136 achievements.

## Downloads

- [Android APK](Magium-Text-Edition-v0.2.15.apk?raw=true)
- [Standalone browser HTML](Magium-Text-Edition-v0.2.15.html?raw=true)
- [Source and rebuild tools](Magium-Text-Source-v0.2.15.zip?raw=true)
- [SHA-256 checksums](SHA256SUMS.txt)

Download the HTML and open it in a browser; GitHub’s file viewer does not run it.

## Changes since 0.2.9

- Correctly load legitimate saves containing temporary Hearing bonuses.
- Preserve book-start saves when returning to checkpoints.
- Keep the Consolation prize death counter cumulative across loads, Back and new games.
- Restore required story Stats screens when loading saved games.
- Associate saves with their checkpoints and repair unsafe legacy death checkpoints.
- Leave the current game unchanged if a save cannot be loaded successfully.
- Preserve damaged saves before overwriting them and identify damaged slots clearly.
- Improve backup export/import, recovery data and warnings when optional history cannot fit.
- Show the native export confirmation inside the Backup window.

The original story, choices and pinned upstream interpreter are retained.
All included books remain unlocked during testing; no purchases are enabled.
The Menu retains the Reddit community link, offline Privacy policy and credits.

## Android updates

Android 8.0 or later; package org.magium.textedition; versionCode 18;
versionName 0.2.15; target SDK 36; launcher label “Magium Text”.

This GitHub APK retains the signing certificate used for previous direct APKs.
Install it as an update over the previous direct Text Edition APK to preserve saves.
Do not uninstall first. Google Play installations use Google Play’s signing key;
update those through Google Play rather than installing this APK over them.
Manual backup export/import is available for transferring progress.
This app is a separate package from Cristian’s original application.

Google Play closed-test invitation:
https://play.google.com/apps/testing/org.magium.textedition
Access requires an eligible Google account on the tester list.

## Validation

All 60 automated regression tests pass. Independent review reproduced the earlier
bugs, checked their corrections, and exercised randomized save/checkpoint and
backup round trips. Flori tested installation over the prior direct APK, preserved
progress/saves/achievements, and actual native backup export/import on a phone.
Version 0.2.15 was also installed through a Google Play update on a separate tester
phone; that phone had no prior progress to test migration.
These checks do not establish that every possible story route has been played.

Low-priority issues remain with full-storage errors during play and technical
error wording; the independently reviewed save/load and backup corrections are
included. No signing keys or passwords are included in the source archive.

## Implementation and credits

This edition uses Thuiop and contributors’ JavaScript interpreter and web
adaptation (MagiumJS), including its parser, execution routines, original stat
and state routines, and achievement metadata. The pinned upstream commit is
51f5aa9406c094e5133be2c7d69988296f86cfbc:
https://github.com/thuiop/magium-dev

- Cristian Mihailescu: story and original game.
- Flori Dumitrescu, Cristian’s mother and sole heir: shared the original source
  and prepared this edition in collaboration with Codex, an OpenAI agent.
- Radu Privantu: created the original open-source repository with her permission:
  https://github.com/raduprv/Magium
- Thuiop: extracted the original text and branching conditions from Cristian’s
  Clickteam project; Thuiop and contributors developed the interpreter and web
  adaptation used here, with community testing.
- dragon_l: acknowledgment for the earlier Android APK.
- Claude: independent review of save, checkpoint and backup behavior.
- EJS 3.1.10, Matthew Eernisse and contributors: offline templates, Apache 2.0.
- Original Magium icon artwork: “Magic Ball” by Agnes Landgraf (Wyonet):
  https://www.deviantart.com/wyonet/art/Magic-ball-362647907

AI assistance was used for the adapted reading interface, offline Android
integration, packaging and verification. Cristian’s original story and the
upstream community implementation are credited separately.

MIT software notices and EJS’s Apache notice are retained in the app and source.
The original repository’s text licensing statement is at:
https://github.com/raduprv/Magium#readme
Icon artwork has separate usage terms. See LICENSE, CREDITS.md, ATTRIBUTION.txt,
ADAPTER.md and vendor notices, also included in the source archive.

No ads, analytics, external fonts, audio or story illustrations are bundled.
