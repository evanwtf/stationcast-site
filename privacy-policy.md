---
layout: default
title: Privacy Policy
permalink: /privacy-policy.html
---

# Privacy Policy for StationCast

**Last Updated: April 3, 2026**

## Introduction

StationCast ("we," "us," "our," or "the App") is committed to protecting your
privacy. This Privacy Policy explains how we collect, use, disclose, and
otherwise handle your information when you use the StationCast mobile
application (the "App") and its associated services.

Please read this Privacy Policy carefully. By downloading and using
StationCast, you agree to the practices described in this policy.

## 1. Information We Collect

### 1.1 Information You Provide Directly

- **Station Configuration**: When you add personal weather stations to the
  App, we store the station identifiers (e.g., Weather Underground station
  IDs) and custom labels or names you assign.
- **Account Information**: If applicable, API keys or authentication
  credentials you provide to access our backend service.
- **Preferences**: Your choices regarding temperature units, wind speed units,
  pressure units, and other display preferences.
- **Custom Labels**: Station labels (e.g., "Home," "Work," "Beach") that you
  create or select.

### 1.2 Location Information

- **Optional Location Access**: When you use the station discovery feature,
  StationCast may request access to your device's location. This is used
  only to:
  - Find nearby personal weather stations and sort them by proximity
  - Display distance information relative to your current location

  Location data is **not sent to our servers** and is **not stored or
  logged** by StationCast. It remains on your device and is used only for
  local proximity calculations.

- **Timezone Detection**: We use your device's timezone setting to display
  station data with correct local times.

### 1.3 Automatically Collected Information

- **App Usage Data**: Crash logs and error reports to help us improve
  stability and performance.
- **Device Information**: Device model, iOS version, and app version (for
  compatibility and debugging).
- **API Requests**: When fetching weather data, our backend logs:
  - Which station IDs you request observations for
  - Timestamps of data fetches
  - Errors or failed requests

  These logs are retained for up to 30 days and help us diagnose service
  issues and track API usage. We do not build query history profiles from
  this data.

## 2. How We Use Your Information

We use the information we collect to:

- **Provide Core Services**: Fetch current and historical weather observations
  from configured stations
- **Improve the App**: Analyze crashes, errors, and usage patterns to improve
  stability and performance
- **Personalization**: Apply your unit preferences and display settings
- **Service Operation**: Manage our backend service, including caching and
  rate limiting
- **Compliance**: Fulfill legal obligations and respond to lawful requests

We do **not** use your information for:

- Selling or sharing your station data or weather preferences with third
  parties for their commercial purposes
- Creating behavioral profiles about you
- Advertising (StationCast does not currently serve ads)

## 3. Third-Party Services

### 3.1 Weather Underground

StationCast fetches weather data from [Weather Underground](https://www.wunderground.com/)
on your behalf. When you use the App:

- Your **station IDs** are sent to Weather Underground's API
- Weather Underground's privacy policy applies to their data collection:
  https://www.wunderground.com/about/privacy

We do not control Weather Underground's privacy practices.

### 3.2 StationCast Backend Service

If you configure the App to use the StationCast backend service (instead of
direct Weather Underground API access):

- Your **station IDs** are sent to our backend
- Our backend caches observations server-side and returns normalized data
- The backend enforces API rate limits and authentication

Backend request logs (station IDs, timestamps, errors) are retained for up to
30 days for troubleshooting purposes, then deleted.

## 4. Advertising

StationCast does not currently display advertisements. If we introduce
advertising in the future, this policy will be updated with full details
before any ads are shown.

## 5. Data Security

We implement reasonable security measures to protect your information:

- **Local Storage**: Station IDs and preferences are stored in the iOS
  Keychain and UserDefaults with standard iOS protections
- **In Transit**: API requests use HTTPS encryption
- **Backend**: Our backend enforces API key authentication; keys are stored
  securely and never transmitted in the URL

No security system is perfectly secure. We cannot guarantee absolute
protection against all possible attacks or unauthorized access.

## 6. Data Retention

- **Station Configuration & Preferences**: Stored locally on your device
  until you delete the App or manually remove stations
- **Cache Data**: Our backend caches observations temporarily (TTL-based)
  to reduce redundant API calls
- **Logs**: Backend request logs are retained for up to 30 days, then
  deleted

When you delete the App, all local data is removed from your device.

## 7. Your Privacy Rights & Choices

### 7.1 Location Permissions

You can grant or deny location access when prompted during station discovery:

- On iOS, visit **Settings > StationCast > Location** to change permissions
  at any time
- If you deny location access, proximity-based station sorting is unavailable,
  but all other features remain functional

### 7.2 Data Deletion

- **Remove Stations**: Delete individual stations in the App's Manage
  Stations view
- **Reset All Data**: Use the Settings > Reset option to clear all stations
  and preferences
- **Uninstall**: Removing the App deletes all local data from your device
- **Backend Data**: Contact us at evandhoffman@gmail.com to request
  deletion of any data associated with your API key

### 7.3 API Keys

If you use the StationCast backend service, you can rotate or revoke your
API key through your account settings, or contact us to request deletion of
associated data.

## 8. Children's Privacy

StationCast is not intended for children under 13. We do not knowingly
collect information from children under 13. If we become aware that a child
under 13 has provided us with information, we will delete it promptly.

## 9. Changes to This Privacy Policy

We may update this Privacy Policy from time to time. We will notify you of
material changes by:

- Updating the "Last Updated" date at the top of this policy
- Posting the revised policy in the App

Your continued use of StationCast after changes are posted constitutes
acceptance of the updated policy.

## 10. Contact Us

**Email**: evandhoffman@gmail.com

We will respond to privacy inquiries within 30 days.

## 11. Additional Information by Jurisdiction

### United States (CCPA / CPRA)

If you are a California resident, you have the right to:

- Know what personal information is collected
- Delete personal information (with certain exceptions)
- Opt-out of the sale or sharing of personal information

We do not sell your personal information.

To exercise these rights, contact us at privacy@stationcast.app.

### European Union (GDPR)

If you are in the EU, your legal bases for processing include:

- **Legitimate Interests**: To operate the App and provide weather services
- **Contract**: To provide the requested weather data fetching service
- **Consent**: For location access (controlled via iOS permissions)

You have the right to access, correct, delete, or port your data, and to
object to processing. To exercise GDPR rights, contact us at
privacy@stationcast.app.

---

**StationCast is a labor of love. We respect your privacy and will never
abuse it.**
