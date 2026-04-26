# Privacy Policy

_Last updated: 26 April 2026_

Traductor is built privacy-first. The short version: **we do not collect,
transmit, or sell any of your data**. Everything you do in the app stays
on your device.

## What data we collect

**None.** Traductor has no analytics, no advertising, no account system,
and no sign-in. We do not see what books you read, what words you save,
how often you open the app, or which device you use it on.

This is declared in the app's `PrivacyInfo.xcprivacy` manifest as
**Data Not Collected**, and matches the App Store privacy questionnaire
answers.

## What stays on your device

The following live entirely in local storage on your iPhone:

- **Imported books** (EPUB and PDF files).
- **Your personal dictionary** — saved words, translations, notes, the
  source sentences they came from, and your mastery state.
- **Reading position** for each book.
- **App preferences** — theme, type size, configured external dictionary
  URL templates.

If you delete the app, this data is removed from your device. There is
no cloud copy, because there is no cloud.

## Translation

Translations are produced **on-device** by Apple's
[Translation framework](https://developer.apple.com/documentation/translation).
No translation request leaves your iPhone, and no third-party translation
service is contacted.

When you first use a language pair, iOS may download a language pack
from Apple. That request goes directly to Apple, not to us, and is
covered by [Apple's privacy policy](https://www.apple.com/legal/privacy/).

## External dictionary lookups

Traductor lets you configure URL templates for external online
dictionaries (Wiktionary, Linguee, Le Robert, Larousse, Duden, RAE,
dict.cc, and any others you add). When you tap "open in dictionary",
the URL is opened in an in-app browser sheet (`WKWebView`).

That request goes directly from your device to the dictionary website
you configured — Traductor's developer does not run a server, does not
proxy the request, and does not see what you looked up. The dictionary
website's own privacy policy applies to anything it logs.

You can edit or remove dictionary URL templates at any time in the app.

## Crash reports and diagnostics

Traductor uses Apple's `MetricKit` to receive aggregate, on-device
performance and crash diagnostics that **you choose to share with
developers** via iOS Settings → Privacy & Security → Analytics &
Improvements → Share With App Developers.

If you have that setting **on**, iOS may send anonymised, aggregated
crash and performance reports to us through Apple's infrastructure. We
use these only to fix bugs. If you have that setting **off** (the iOS
default), nothing is sent.

We do not bundle any third-party crash-reporting or analytics SDK.

## Children

Traductor is rated 4+ and contains no advertising, no in-app purchases,
no social features, and no user-generated content. The app does not
collect any data from anyone, including children.

## Changes to this policy

If this policy ever changes, the updated version will be published at
this URL with a new "Last updated" date. Material changes will be
called out in the app's release notes.

## Contact

Questions about privacy? Email **hardyharsh82@gmail.com**.
