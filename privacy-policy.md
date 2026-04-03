# Privacy Policy for StationCast

**Last Updated: April 3, 2026**

## Introduction

StationCast ("we," "us," "our," or "the App") is committed to protecting your privacy. This Privacy Policy explains how we collect, use, disclose, and otherwise handle your information when you use the StationCast mobile application (the "App") and its associated services.

Please read this Privacy Policy carefully. By downloading and using StationCast, you agree to the practices described in this policy.

## 1. Information We Collect

### 1.1 Information You Provide Directly

- **Station Configuration**: When you add personal weather stations to the App, we store the station identifiers (e.g., Weather Underground station IDs) and custom labels or names you assign.
- **Account Information**: If applicable, API keys or authentication credentials you provide to access our backend service.
- **Preferences**: Your choices regarding temperature units, wind speed units, pressure units, and other display preferences.
- **Custom Labels**: Station labels (e.g., "Home," "Work," "Beach") that you create or select.

### 1.2 Location Information

- **Optional Location Access**: When you use the station discovery feature, StationCast may request access to your device's location. This is used only to:
  - Find nearby personal weather stations and sort them by proximity
  - Display distance information relative to your current location
  
  Location data is **not sent to our servers** and is **not stored or logged** by StationCast. It remains on your device and is used only for local proximity calculations.

- **Timezone Detection**: We use your device's timezone setting to display station data with correct local times.

### 1.3 Automatically Collected Information

- **App Usage Data**: Crash logs and error reports to help us improve stability and performance.
- **Device Information**: Device model, iOS version, and app version (for compatibility and debugging).
- **API Requests**: When fetching weather data, we log:
  - Which station IDs you request observations for
  - Timestamps of data fetches
  - Errors or failed requests
  
  These logs help us diagnose service issues and track API usage.

### 1.4 Advertising Information (Current & Future)

Currently, StationCast does not display advertisements. However, we may introduce advertising in the future. If we do:

- **Ad Network Data**: We may partner with third-party ad networks (e.g., Google AdMob, Meta Audience Network) that collect:
  - Device identifiers (e.g., IDFA)
  - Approximate location (city/region level, not precise GPS)
  - App usage patterns and engagement data
  - Device information
  
- **Behavioral Targeting**: Ad networks may use this data to show you personalized ads based on your interests
- **Ad Measurement**: We and our ad partners may track ad impressions, clicks, and conversions

Any advertising implementation will be clearly disclosed in the App and in this Privacy Policy with full details about which ad networks are used.

## 2. How We Use Your Information

We use the information we collect to:

- **Provide Core Services**: Fetch current and historical weather observations from configured stations
- **Improve the App**: Analyze crashes, errors, and usage patterns to improve stability and performance
- **Personalization**: Apply your unit preferences and display settings
- **Service Operation**: Manage our backend service, including caching and rate limiting
- **Advertising** (if enabled): Serve ads through third-party ad networks and measure ad performance
- **Compliance**: Fulfill legal obligations and respond to lawful requests

We do **not** use your information for:
- Selling or sharing your station data or weather preferences with third parties for their commercial purposes
- Creating detailed behavioral profiles about you independent of advertising
- Cross-app tracking beyond what ad networks do for their own purposes

## 3. Third-Party Services

### 3.1 Weather Underground

StationCast fetches weather data from [Weather Underground](https://www.wunderground.com/) on your behalf. When you use the App:

- Your **station IDs** are sent to Weather Underground's API
- Weather Underground's privacy policy applies to their data collection: https://www.wunderground.com/about/privacy

We do not control Weather Underground's privacy practices. Review their privacy policy for details on how they handle your requests.

### 3.2 StationCast Backend Service

If you configure the App to use the StationCast backend service (instead of direct Weather Underground API access):

- Your **station IDs** are sent to our backend
- Our backend caches observations server-side and returns normalized data
- The backend enforces API rate limits and authentication

We store only the data necessary to serve observations; we do not retain historical logs of which stations you query.

## 4. Data Security

We implement reasonable security measures to protect your information:

- **Local Storage**: Station IDs and preferences are stored in the iOS Keychain and UserDefaults with standard iOS protections
- **In Transit**: API requests use HTTPS encryption
- **Backend**: Our backend enforces API key authentication; keys are stored securely and never transmitted in the URL

However, no security system is perfectly secure. We cannot guarantee absolute protection against all possible attacks or unauthorized access.

## 5. Data Retention

- **Station Configuration & Preferences**: Stored locally on your device until you delete the App or manually remove stations
- **Cache Data**: Our backend caches observations temporarily (TTL-based) to reduce redundant API calls
- **Logs**: API request logs are retained for up to 30 days for troubleshooting and billing purposes

When you delete the App, all local data is removed from your device.

## 6. Your Privacy Rights & Choices

### 6.1 Location Permissions

You can grant or deny location access when prompted during station discovery:
- On iOS, visit **Settings > StationCast > Location** to change permissions at any time
- If you deny location access, the App will not use proximity-based station sorting, but other features remain available

### 6.2 Data Deletion

- **Remove Stations**: Delete individual stations in the App's Manage Stations view
- **Reset All Data**: Use the Settings > Reset option to clear all stations and preferences
- **Uninstall**: Removing the App deletes all local data from your device

### 6.3 API Keys

If you use the StationCast backend service, you can:
- Rotate or revoke your API key through your account settings (when available)
- Contact us (see Section 8) to request deletion of associated data

### 6.4 Advertising Preferences

If StationCast includes ads:

- **Limit Ad Tracking**: On iOS, you can limit personalized ads by:
  - Going to **Settings > Privacy > Apple Advertising** and enabling "Limit Ad Tracking"
  - Going to **Settings > Apps > StationCast > App Tracking Transparency** and denying permission
  
- **Remove Ads**: Some future versions of StationCast may offer a premium ad-free subscription or one-time purchase to remove ads entirely
- **Opt-Out of Behavioral Ads**: You can opt out of personalized advertising by adjusting your iOS privacy settings, though you may still see non-personalized ads

Ad networks are required to honor these settings; however, we recommend reviewing the privacy policies of the specific ad networks in use for complete details on their practices.

## 7. Children's Privacy

StationCast is not intended for children under 13 (or the applicable age of digital consent in your jurisdiction). We do not knowingly collect information from children under 13. If we become aware that a child under 13 has provided us with information, we will take steps to delete such information and terminate the child's account.

## 8. Changes to This Privacy Policy

We may update this Privacy Policy from time to time to reflect changes in our practices, technology, legal requirements, or other factors. We will notify you of material changes by:
- Updating the "Last Updated" date at the top of this policy
- Posting the revised policy in the App

Your continued use of StationCast after changes have been posted constitutes your acceptance of the updated Privacy Policy.

## 9. Contact Us

If you have questions about this Privacy Policy, wish to exercise your privacy rights, or want to report a privacy concern, please contact us:

**Email**: privacy@stationcast.app

**Mailing Address**:
StationCast
[Address TBD]

**Response Time**: We will respond to privacy inquiries within 30 days.

## 10. Additional Information by Jurisdiction

### United States (CCPA / CPRA)

If you are a California resident, you have the right to:
- Know what personal information is collected
- Delete personal information (with certain exceptions)
- Opt-out of the sale/sharing of personal information (we do not sell your station data; ad networks may use data for their own purposes)

If StationCast includes ads, data shared with ad networks may be considered "sharing for cross-context behavioral advertising." You can limit this by disabling app tracking via iOS Settings.

To exercise these rights, contact us at privacy@stationcast.app.

### European Union (GDPR)

If you are in the EU, your legal basis for processing includes:
- **Legitimate Interests**: To operate the App and provide weather services
- **Contract**: To provide the requested weather data fetching service
- **Consent**: For location access (you control this via iOS permissions) and for personalized advertising (if implemented)

If StationCast includes ads, we will obtain your explicit consent before sharing data with ad networks for personalized advertising. You may withdraw consent at any time via iOS Settings.

You have the right to:
- Access your information
- Correct inaccurate data
- Request deletion ("right to be forgotten")
- Port your data
- Object to processing and profiling for ads

To exercise GDPR rights, contact us at privacy@stationcast.app.

---

**StationCast is a labor of love. We respect your privacy and will never abuse it.**
