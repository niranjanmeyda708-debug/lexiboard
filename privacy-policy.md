---
title: LexiBoard Privacy Policy
---

# LexiBoard Privacy Policy

**Effective date:** [15-10-2026]
**Applies to:** the LexiBoard Android keyboard application (`com.lexiboard`)

LexiBoard is an independent, open-source keyboard for Android, built on the FlorisBoard project.
This policy explains, in plain terms, what the app does with your data. The short version: the
keyboard works on your device and does not collect anything for us. The **only** time text leaves
your device is when you deliberately use one of the optional AI features, and then it goes to the
AI provider you configure — never to a server we run.

If any statement here does not match what you observe the app doing, please tell us (see
[Contact](#contact)); that is a bug, and we will fix either the app or this document.

## Who we are

LexiBoard is published by **[NM.Co]**. The data controller
for this app is that publisher. Contact: **[niranjanmeyda708@gmail.com]**.

## What stays on your device

Everything below is stored only in the app's private storage on your phone and is never uploaded by
LexiBoard:

- **What you type.** The keyboard learns from and completes your input on the device. Typing data
  is not transmitted.
- **Clipboard history, emoji history, and your personal dictionary.**
- **Your settings** — themes, layouts, languages, gestures, and the AI options described below.
- **Your AI provider API key**, if you enter one.
- **Crash reports.** If the app crashes, it can show you a local crash dialog and write a log to the
  app's private storage. Nothing is uploaded automatically.
- **Screen text read by the screen translator** is processed by an on-device OCR engine (Google ML
  Kit, with the language models bundled inside the app). The image never leaves the device; only the
  recognised text can leave, and only as described below.

LexiBoard contains **no advertising, no analytics, no crash-reporting SDK, and no third-party
tracking of any kind**. It has no user accounts and does not ask you to log in.

## What is sent off your device, and when

There are exactly two situations in which LexiBoard itself sends anything over the network. Both
require a deliberate action by you.

### 1. The AI features (Rephrase, Translate, and the screen translator)

These features are **off until you explicitly agree**, on a dedicated consent screen shown the first
time you start one of them. When you agree and then use a feature, the app sends the relevant text
over an encrypted (HTTPS) connection to your configured AI provider:

- **Rephrase / Translate** send the sentence at your cursor, or the text you have selected.
- **The screen translator** sends the text its on-device OCR read from the area you framed.
- **The translate share target** sends the text you chose to share into LexiBoard.

That text is sent to the **AI provider you configure in AI settings**. By default the app is set up
to use the [AIRouter](https://airouter.in) gateway (`api.airouter.in`), which forwards your request
to a language model and returns the result. Your **API key** is sent with each request so the
provider can authorise it. LexiBoard operates no server of its own and keeps no copy of your text or
your key anywhere but your device.

Once the text reaches your provider, that provider's own privacy policy governs what it does with
it. AIRouter is a separate company; please review its terms and privacy policy, and choose a
provider whose handling of your text you are comfortable with.

You can **withdraw consent at any time** in AI settings → Data and privacy. Withdrawing stops all of
these features from sending anything.

### 2. Checking for extension updates

FlorisBoard supports community extensions (keyboard layouts, themes, emoji packs). If you open the
extensions screen and tap **Check for updates**, the app sends the list of extensions you have
installed — their package identifiers and versions — to the FlorisBoard addons store
(`beta.addons.florisboard.org`) to ask whether newer versions exist. This is a feature of the
upstream FlorisBoard project and does not involve LexiBoard's publisher. No text you have typed is
included. If you never tap that button, nothing is sent.

## Permissions and why they exist

| Permission | Why the app asks for it |
| --- | --- |
| Internet | To reach your AI provider for the AI features, and the addons store for extension updates. |
| Vibrate | Haptic feedback on key press, if you enable it. |
| Post notifications | To show the foreground notification required while the screen translator is capturing the screen. |
| Draw over other apps | To show the screen-translator viewfinder over the app you are translating. |
| Foreground service / media projection | To capture the screen region you frame for the screen translator. Capture runs only while you use the feature and stops when you close it. |

## Data retention

LexiBoard's publisher retains **no** personal data, because none is sent to us. Data held on your
device persists until you clear it (or uninstall the app). Text sent to your AI provider is retained
according to that provider's policy, which we do not control.

## Security

All network traffic from the app uses HTTPS. Your API key is stored in the app's private storage.
No method of transmission or storage is perfectly secure, but we have designed the app so that the
sensitive material — your typing and your key — stays on your device by default.

## Children

LexiBoard is a general-purpose keyboard and is not directed at children. It does not knowingly
collect personal information from anyone, including children.

## Changes to this policy

If this policy changes, the new version will be published at this URL with a new effective date.
Material changes will also be noted in the app's changelog.

## Contact

Questions or concerns about this policy or the app's data practices:
**[niranjanmeyda708@gmail.com]**.

## Open source

LexiBoard is built on [FlorisBoard](https://florisboard.org), which is free and open-source software.
The app's source code is available in the project repository, so you can verify the behaviour
described in this policy for yourself.
