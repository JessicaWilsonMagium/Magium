# Magium — Text Edition 0.2.9

Offline Android and browser edition of Cristian Mihailescu’s original interactive
Books 1–3: 34 chapters, 2,159 scenes and 136 achievements.

## Downloads

- [Android APK](Magium-Text-Edition-v0.2.9.apk?raw=true)
- [Standalone browser HTML](Magium-Text-Edition-v0.2.9.html?raw=true)
- [Source and rebuild tools](Magium-Text-Source-v0.2.9.zip?raw=true)
- [SHA-256 checksums](SHA256SUMS.txt)

Download the HTML and open it in a browser; GitHub’s file viewer does not run it.

## Changes in 0.2.9

The visible in-game Credits now explicitly acknowledge Thuiop and contributors
for the JavaScript interpreter and web adaptation (MagiumJS), including the
parser, interpreter, original stat/state routines and achievement metadata.
The original source extraction credit and licence notices are retained.

## Retained from 0.2.8

The Menu includes an offline Privacy policy covering local saves, manual backup
files, support emails and external links. The same policy is published at:
https://jessicawilsonmagium.github.io/Magium/privacy-policy.html

## Retained from 0.2.7

The in-game credits now explicitly acknowledge extraction of Cristian’s original
text and branching conditions by Thuiop. The Android launcher label remains
“Magium Text”, independently of the longer Google Play listing title.

## Retained from 0.2.6

The Menu now includes “Magium community on Reddit”, linking to
https://www.reddit.com/r/Magium/best/ . It follows the current reading theme.
Source credits now clarify that Flori Dumitrescu shared Cristian’s original
source and Radu Privantu created the open-source repository with her permission.

The original-style achievement cards, book/chapter progress counters, three
reading themes, adjustable font and text size, 30 named saves, checkpoints,
backup export/import, normal Back navigation and original story are retained.
All included books remain unlocked during testing; no purchases are enabled.

## Android updates

Android 8.0 or later; package org.magium.textedition; versionCode 12;
versionName 0.2.9; target SDK 36. Install over the existing Text Edition to keep
its saves. Do not uninstall first. This is a separate package from Cristian’s
original application. The existing signing certificate, native DEX, asset origin
and save namespaces are retained.

Prepared on 22 October 2026. Closed testing Alpha version 11 (0.2.8) was
published on Google Play on 21 October; internal testing remains 10 (0.2.7).
This version 12 (0.2.9) is prepared for upload and has not been submitted to Play.
A separate intellectual-property documentation clarification is pending with
Google support. No tester recruitment announcement has been posted.

## Implementation and validation

This edition uses Thuiop and contributors’ existing parser, execution routines
and story data, pinned at 51f5aa9406c094e5133be2c7d69988296f86cfbc:
https://github.com/thuiop/magium-dev

AI assistance was used for the reading interface, offline integration,
verification and Android packaging. This does not make the upstream work
AI-created. See ADAPTER.md for boundaries and the two compatibility corrections.

Version 0.2.9 passes 21 existing regression checks, APK offline-startup and
save/reload checks, original runtime/DEX/asset integrity checks, original signer
verification and official bundletool validation. The earlier Reddit menu link was checked at 390×844 in all three themes.
The Privacy policy opens and closes offline in the packaged app smoke
check without changing the game state. This is a jsdom check, not an Android
device execution test.
These checks do not replace a physical Android acceptance test; the new build
has not yet been reviewed on a phone.

The source contains the pinned native DEX and APK/AAB packaging tools. It does
not reconstruct that DEX. Signing keys and passwords are not included.

## Credits and licences

- Cristian Mihailescu: story and original game.
- Flori Dumitrescu, Cristian’s mother and sole heir: shared the original source
  and prepared this edition in collaboration with Codex, an OpenAI agent.
- Radu Privantu: created the original open-source repository with her permission:
  https://github.com/raduprv/Magium
- Thuiop and contributors: existing web adaptation, parser, runtime, data,
  stat/state routines, achievement metadata and community testing.
- dragon_l: acknowledgment for the earlier Android APK; this does not attribute
  our Android wrapper to him.
- EJS 3.1.10, Matthew Eernisse and contributors: offline templates, Apache 2.0.
- Original Magium icon artwork: “Magic Ball” by Agnes Landgraf (Wyonet):
  https://www.deviantart.com/wyonet/art/Magic-ball-362647907

The original source repository explicitly identifies story data as CC BY 4.0:
https://creativecommons.org/licenses/by/4.0/
MIT software notices and EJS’s Apache notice are retained. Icon artwork has
separate usage terms and is not represented as covered by those licences.
See LICENSE, CREDITS.md, ATTRIBUTION.txt and vendor notices.

No ads, analytics, external fonts, audio or story illustrations are bundled.
