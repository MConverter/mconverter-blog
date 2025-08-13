---
title: Important information for iOS users in the EU
description: Apple was about to break installable web apps in iOS 17.4, leading to local data loss. See what would've changed and why.
image: web_app_open_in_browser.webp
image_alt: Screenshot of iPhone showing that “MConverter” will open in your default browser from now on
date_added: 2024-02-23
date_updated: 2024-03-06
categories:
  - help
  - technical
aside_cards:
  - mobile_app
---

*Thanks to a potential [formal investigation](https://www.ft.com/content/d2f7328c-5851-4f16-8f8d-93f0098b6adc) by the European Commission and an [open letter](https://letter.open-web-advocacy.org/) to Tim Cook, Apple has reversed its decision to disable installable web apps in the EU.*

*Our original article follows.*

---

In the coming weeks, with the release of iOS 17.4, you may see the following message if you have MConverter installed (added to your home screen): **“MConverter” will open in your default browser from now on.**

Due to Apple's changes, MConverter will no longer open as a web app that appears in the app switcher. Instead, it will load as a regular website in your default browser.

## Will I lose functionality or any data?

We are doing everything possible to keep all existing functionality on iOS. Unfortunately, Apple's last-moment and [mostly undocumented](https://www.theregister.com/2024/02/16/apple_web_apps/) changes offer no replacements for some features. **The following functionality will be impacted**:

* Push notifications
* Local MConverter settings
* Keeping you logged in

### Push notifications when a conversion is done or in progress

iOS is the only platform where web push notifications are available [only for web apps added to your home screen](https://caniuse.com/push-api#:~:text=WKWebView%20nor%20SFSafariViewController-,6,Requires%20website%20to%20first%20be%20added%20to%20the%20Home%20Screen.,-Delivered%20silently%2C%20meaning), and not for websites. Because MConverter will now load as a website in your browser, **you will no longer receive notifications about your file conversions**.

Apple does not offer any way for us to make this functionality available again on iOS.

### Intelligent Tracking Prevention and its unintended consequences

Websites that open in your browser are subject to Apple's *Intelligent Tracking Prevention* which automatically [deletes all local data](https://webkit.org/tracking-prevention/#:~:text=to%2024%20hours.-,7%2DDay%20Cap%20on%20All%20Script%2DWriteable%20Storage,-Trackers%20executing%20script) for websites you haven't visited in the last 7 days.

These protections cause unintended consequences and may negatively impact your experience with MConverter. Specifically, if you do not visit the MConverter website for more than 7 days, **your local settings will be reset and deleted by iOS**. These settings include:

* whether to automatically download your converted files;
* whether to remove the \[MConverter.eu\] branding from file names;
* whether to convert files on-device if possible;
* your dark/light mode preferences;
* your accessibility preferences for reduced motion;
* your recently used file formats, if not logged in.

Moreover, Apple's restrictions mean that you will need to **log into your MConverter account again whenever more than 7 days have passed** since your last usage.

As you may have noticed from before, web apps added to home screen do not have such restrictions. Your settings would have been retained indefinitely.

### Isolated local data storage for installed web apps

Local data and cookies on iOS are isolated between your browser and home screen web apps. When your device updates to iOS 17.4 and the transition occurs, all aforementioned MConverter **settings will be lost**. If you use an MConverter account, you will need to **log in again**.

## Which devices and platforms will be impacted?

These changes affect only [iPhone and iPad devices in the EU](https://www.apple.com/newsroom/2024/01/apple-announces-changes-to-ios-safari-and-the-app-store-in-the-european-union/).

All other devices and platforms will keep all existing features of MConverter: macOS, Android, Windows, Linux, ChromeOS, etc.

## Why are these changes happening?

The [Digital Markets Act](https://commission.europa.eu/strategy-and-policy/priorities-2019-2024/europe-fit-digital-age/digital-markets-act-ensuring-fair-and-open-digital-markets_en) (DMA) in the European Union aims to prevent gatekeepers, such as Apple and Google, from abusing their market power by enforcing a set of rules. For example, gatekeepers must allow third-party interoperability, such as full support for third-party browser engines. These changes aim to create a fairer business environment for business users dependent on gatekeepers, provide new opportunities for innovators and startups, and offer consumers more and better services, including the ability to switch providers more easily.

Unfortunately, Apple's way of complying with the new regulations can be seen as hostile and anti-consumer. The DMA does not force Apple to break home screen web apps. The decision to remove them entirely, rather than adapt, looks like a [deliberate choice to reduce functionality](https://open-web-advocacy.org/blog/apple-on-course-to-break-all-web-apps-in-eu-within-20-days/) and, ironically, *limit* user choice.

Apple cites security and privacy concerns as the reason for removing home screen web apps on iOS. However, other operating systems, *including macOS*, already have installable web apps and third-party browser engine support. Therefore, the excuse for iOS seems questionable.

## I don't like these changes. What can I do?

If you're a user, [let Apple know](https://feedbackassistant.apple.com/) that you'll be negatively impacted.

If you are a developer, the Open Web Advocacy organization is collecting evidence from impacted businesses and developers. OWA will submit this feedback to the European Commission. We recommend that you join us in filling out their survey: [https://open-web-advocacy.org/apple-attempts-killing-webapps/](https://open-web-advocacy.org/apple-attempts-killing-webapps/)