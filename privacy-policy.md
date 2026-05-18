---
layout: default
title: Privacy Policy
permalink: /privacy-policy.html
---

# Privacy Policy

<p class="page-meta">Last Updated: May 18, 2026</p>

## Introduction

StationCast ("we," "us," "our," or "the App") is a personal weather station companion. This Privacy Policy explains what information we handle when you use the StationCast iOS app, the iOS widget extension, and the StationCast backend service that the app talks to. It also covers the optional Amazon Alexa skill, when you choose to enable it.

By using StationCast, you agree to the practices described here.

## Intended audience and GDPR notice

StationCast is intended for users in the United States. The service is **not directed at users in the European Union, the United Kingdom, or other jurisdictions with comparable data-protection regimes** (including but not limited to the EU GDPR and the UK GDPR).

**StationCast is not GDPR-compliant or UK-GDPR-compliant.** We have not built the processes, documentation, controls, or compliance infrastructure required by those regimes, and we will not honor data-subject access, deletion, portability, restriction, objection, or transfer requests made under those regimes. We have no Data Protection Officer, no EU representative, no international-transfer safeguards, and no automated retention or deletion processes.

**If you are a resident of the EU, the UK, or any other jurisdiction with a comparable data-protection regime, please do not use StationCast.** We do not technically block access. If you choose to use the app despite this notice, you acknowledge that the app is not GDPR / UK GDPR compliant, that we will not accommodate GDPR / UK GDPR rights or obligations on your behalf, and that you use the app on that basis.

## 1. Information we handle

### 1.1 Information you provide

- **Personal weather station configuration.** When you save a station, we store its station identifier and any custom label you assign (for example, "Home," "Mom's," "Beach"). Custom labels are short freeform strings you choose; we do not derive meaning from them.
- **Preferences.** Your display choices — temperature, wind speed, pressure, and distance units; map label configuration; initial map radius; launch behavior; share-image QR code on/off; sparkline visibility; iPad sidebar default; and similar settings.
- **Photos library, only when you ask.** If you tap "Save to Photos" on a share image, iOS prompts you for permission to add an image to your library. We never read your photo library.
- **Amazon Alexa account linking (optional).** If you choose to enable the StationCast Alexa skill, the standard OAuth 2.0 account-linking flow runs against our backend. We store the link between your Amazon-side identifier and which StationCast station(s) you've linked to it, plus any nickname you assigned and which one (if any) is your default. We hash the Amazon-supplied user identifier before logging it so it does not appear in plain text in our logs. You can unlink the skill at any time from the Alexa app; see [Section 7](#7-your-privacy-rights--choices) for what happens to the server-side record.

### 1.2 Location, only with your permission

The app requests your device's location (when-in-use) for these purposes:

- **Discovery**: finding personal weather stations near you and sorting them by distance.
- **Distance display**: showing how far each saved station is from your current location.
- **Auto-select nearest saved station on launch**: if you enable this in Settings, the app opens to whichever of your saved stations is geographically closest to you.
- **Saved-station map framing**: centering the saved-station map on your current location when you open it.
- **Timezone**: we use your device's timezone setting to render observation times correctly.

Location access is optional. If you decline, every feature still works except the four bullets above. Your location is used on-device for the features that need it; the backend receives station identifiers, not your coordinates. (Discovery and "nearby" searches do send a center latitude and longitude to the backend so it can find stations near a point — that's the one path where a location coordinate leaves the device, and it only happens for that specific search.)

### 1.3 Information collected automatically

When the app talks to our backend, the backend records server-side log lines containing:

- HTTP method, path, response status, and request duration.
- Your IP address (the immediate peer IP, plus the forwarded chain if you reach us through a proxy or VPN).
- The User-Agent string sent by iOS.
- The StationCast app version, build number, commit short hash, platform (`ios`), and device class (for example, `phone`, `pad`).
- A masked identifier for the credential the request was authenticated with (a prefix of the API key hash, or the App Attest key identifier — never the secret itself).
- Whether App Attest verification passed.
- The station identifier(s) the request asked about, when the request is for station data.

These logs help us diagnose service problems, detect abuse, and understand which app versions are in the field. We do not build behavioral profiles of individual users from them.

The app does **not** ship a third-party crash reporter or analytics SDK. We do not run Sentry, Firebase, Crashlytics, MetricKit, or comparable telemetry. Apple-platform crash reports may be available to us through App Store Connect if you have opted into "Share With App Developers" in your iOS settings, but that is an Apple-controlled feature; we never collect or transmit crash data ourselves.

## 2. How we use the information

We use the information described above to:

- Provide the core service: fetching, normalizing, and caching weather observations from the stations you've configured.
- Operate the backend: rate-limiting upstream calls, serving cached data when upstream providers are degraded, and authenticating clients.
- Diagnose problems and improve reliability.
- Apply your unit and display preferences.
- Operate the optional Alexa skill, when you've linked it.
- Comply with the law and respond to lawful requests.

We do **not** use the information to:

- Sell or share your saved-station list, weather preferences, or location with third parties for their commercial purposes.
- Build behavioral profiles or marketing audiences.
- Serve advertising. The app currently shows no ads. If that ever changes, this policy will be updated first.

## 3. Third parties involved in providing the service

### 3.1 StationCast backend service

The iOS app does not talk to weather data providers directly. Every request — saved-station observations, nearby search, station discovery, the Alexa skill — goes to our backend, which then mediates with the appropriate upstream. Our backend handles caching, rate limiting, plausibility checks on sensor data, and authentication.

### 3.2 Weather Underground

The current upstream personal-weather-station provider is Weather Underground. When you view a station, our backend may call Weather Underground on your behalf to retrieve current and recent observations for that station identifier. Weather Underground sees the station identifier and our backend's IP, not your device's IP or any identifier specific to you. We cache observations server-side to reduce the number of upstream calls.

### 3.3 Apple App Attest

To stop unauthorized clients from impersonating the app, StationCast uses Apple's App Attest service. On first launch, the app asks Apple to generate a hardware-backed key for this installation of the app. It exchanges a challenge with our backend and the corresponding attestation object is verified against Apple's certificate chain. Our backend stores the resulting public key and a key identifier so it can verify subsequent requests; the private key never leaves your device's Secure Enclave. Subsequent authenticated requests carry a signed assertion that our backend checks. App Attest is an Apple-operated service; please see Apple's privacy policy for what Apple does with the attestation data it processes.

### 3.4 Amazon Alexa (only if you enable the skill)

If you enable the StationCast Alexa skill and link your accounts, Amazon's Alexa service will send signed requests to our backend each time you ask Alexa about a StationCast station. Those requests include an Amazon-supplied user identifier and the spoken intent (for example, "what's the temperature at home"). We use those to look up the station(s) you've linked, fetch their observations through our backend, and return a spoken response. Amazon's handling of your voice data is governed by Amazon's privacy policy; we never receive raw audio. Hosting and account-linking server-side data lives in our backend; see [Section 7](#7-your-privacy-rights--choices) for how to unlink and request deletion.

## 4. Advertising

StationCast does not display advertisements and we do not work with advertising networks. If that changes, this policy will be updated with full details before any ads are shown.

## 5. Authentication and security

We use standard transport security and Apple platform features to protect what's collected:

- **In transit**: all backend traffic uses HTTPS.
- **On device**:
  - Your saved-station list, station labels, and preferences are stored in iOS `UserDefaults` (the standard preferences store), including an App Group container shared with the home-screen widget.
  - The App Attest key identifier — the only sensitive item — is stored in the iOS Keychain.
  - The app's bundled backend API key is shipped inside the app binary, not provided by you, and is used as a fallback while App Attest is still setting up on a fresh install.
- **In the backend**: requests are authenticated with an App Attest assertion when possible, with an API key as fallback. Attested device public keys are stored server-side so we can verify your subsequent requests. Secrets used for signing Alexa OAuth tokens are kept out of logs.

No system is perfectly secure. We cannot guarantee absolute protection against every possible attack.

## 6. Where information is stored

- **On your device**: saved-station list, station labels, preferences, the App Attest key identifier, and the locally-cached observation that powers the widget. Deleting the app removes all of this.
- **On our backend**: the App Attest device public key registered for your installation, transient cached observations for stations users have queried, server-side log lines as described in [Section 1.3](#13-information-collected-automatically), and (only if you've enabled the Alexa skill) the link records described in [Section 1.1](#11-information-you-provide). We do not currently run an automated time-based deletion process for log lines or registered device keys; if you want yours removed, see [Section 7](#7-your-privacy-rights--choices).

## 7. Your privacy rights & choices

### 7.1 Location permissions

You can grant or revoke location access at any time in iOS Settings → StationCast → Location. If you deny location access, every feature continues to work except the location-dependent ones called out in [Section 1.2](#12-location-only-with-your-permission).

### 7.2 Removing stations and resetting the app

- **Remove a single station**: open Manage Stations and delete the station.
- **Reset all stations and preferences**: open Settings and tap "Reset Preferences" at the bottom of the screen.
- **Uninstall**: removing the app from your device deletes everything stored on-device.

### 7.3 Unlinking the Alexa skill

In the Amazon Alexa app, go to Skills & Games → Your Skills → StationCast → Disable Skill. That disables the skill on your Amazon account. To also have the server-side link record (Amazon user hash, linked station identifiers, nickname) removed from our backend, email us per [Section 10](#10-contact-us) — we do not currently provide a self-serve deletion tool for that record.

### 7.4 App Attest device key

If you want the App Attest device record we hold for your installation removed from our backend, email us per [Section 10](#10-contact-us). Removing it means your installation will re-attest on the next request.

## 8. Children's privacy

StationCast is not intended for children under 13. We do not knowingly collect information from children under 13. If we become aware that a child under 13 has provided us with information, we will remove it.

## 9. Changes to this Privacy Policy

We may update this policy from time to time. Material changes are signaled by updating the "Last Updated" date at the top. Your continued use of StationCast after a change is posted constitutes acceptance of the updated policy.

## 10. Contact us

**Email**: evandhoffman@gmail.com

We respond to privacy inquiries as quickly as practical.

## 11. California residents (CCPA / CPRA)

If you are a California resident, you have the right to:

- Know what personal information is collected.
- Request deletion of personal information (with the usual statutory exceptions).
- Opt out of the sale or sharing of personal information for cross-context behavioral advertising.

We do not sell your personal information and we do not share it for cross-context behavioral advertising.

To exercise these rights, contact us at evandhoffman@gmail.com.

---

**StationCast is a labor of love. We respect your privacy and will never abuse it.**
