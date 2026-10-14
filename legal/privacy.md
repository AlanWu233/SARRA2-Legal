# Privacy Policy

**Application:** SARRA2 App  
**Effective Date:** October 14, 2026  
**Last Updated:** October 14, 2026  


## 1. Introduction

Welcome to SARRA2 App.

SARRA2 App (the **“App”**) is an independently developed third-party application designed to provide a simpler, more convenient, and user-friendly experience for accessing the SARRA2 system at Asia-Pacific International University (**“APIU”**).

We recognize the importance of protecting personal information and respecting user privacy. This Privacy Policy describes how the App accesses, processes, stores, and shares information when you use its features and services. It also explains available privacy choices and the limits of the App’s control over information managed by other services.

**SARRA2 App is not an official application of Asia-Pacific International University.** The App operates independently from the university. Access to official university information remains subject to the university’s systems, policies, and applicable terms.

Using the App may involve the processing described here. Where applicable law requires separate consent, this policy does not replace that consent.

## 2. Scope of This Privacy Policy

This Privacy Policy applies to the App and its associated components, where available, including:

- iOS and iPadOS applications;
- Android applications;
- Chrome browser extensions; and
- supporting application-configuration and examination-information services.

Features and technical implementations differ across platforms and versions. The information handled may therefore depend on your device, operating system, enabled features, and settings.

This policy does not replace the privacy policies of APIU or of independent external services accessed through the App.

## 3. Information We Access and Process

### 3.1 Account and Authentication Information

When you sign in, the App may process your university username and password, authentication cookies, session information, security verification tokens, and related authentication or verification information.

This information is used to establish or maintain access to SARRA2. In the normal login flow identified by the reviewed source code, login submissions are directed to the university’s system rather than to a developer-operated student authentication server.

Depending on the platform and your settings, login credentials and session information may be retained on your device as explained in Section 5.

### 3.2 Personal and Academic Information

Depending on what is available in your university account and which features you use, the App may access and process:

- student identification details, name, contact details, and profile information;
- registered courses, academic schedules, grades, GPA, and other academic records;
- class, event, and chapel attendance information;
- examination schedules and related course information;
- university messages and message participants;
- invoices, payment-related information, and other financial records;
- identification-card information; and
- other information provided through the university’s SARRA2 pages or services.

Some university records can contain sensitive information, such as bank account details, nationality, religious information, passport and visa records, and immigration-related information. The App may display or locally cache fields available from the university service. Not every account includes every listed field.

### 3.3 Device and Technical Information

Some functions may process operating-system information, application version, device capabilities, request metadata, and temporary identifiers. Network-service providers can ordinarily receive connection metadata, such as an IP address and standard request headers, when your device contacts their services.

Certain optional remote translation paths may send operating-system details or process-level identifiers to the selected translation service.

### 3.4 Information You Choose to Provide

Additional information may be processed when you fill in university forms, translate a message, save or share a document, configure an external translation endpoint, export diagnostics, or contact the developer for support.

Shared documents, screenshots, message text, or diagnostic reports may contain personal information. Please review them before sharing.

## 4. How Information Is Used

The App processes information as needed to provide or support features such as university sign-in, academic and campus information display, examination matching, saved sessions, local preferences, optional translations, document sharing, and diagnostic troubleshooting.

Some interaction information, including frequently used menu items and recently accessed content, may be kept locally to customize the interface.

The reviewed application code did not show a dedicated developer-operated remote behavioral-analytics or advertising system. This observation does not describe every possible logging or analytics practice of APIU, Cloudflare, operating systems, browsers, or optional outside services.

## 5. Authentication and Credential Storage

### 5.1 iOS and iPadOS

On iOS and iPadOS, the App may store credentials and university authentication cookies using Apple Keychain and browser website storage.

In the reviewed implementation, enabling **Keep me signed in**, password remembering, or multiple-account functionality can cause a password usable for a later sign-in to be saved in Keychain. **Keep me signed in is enabled by default** in that implementation. The stored password is not merely a password hash and the feature should not be understood as keeping cookies only.

The App uses Apple’s platform credential-protection mechanisms, but these do not eliminate all security risks associated with an accessible or shared device.

### 5.2 Android

On Android, the reviewed implementation enables **Remember** by default. When it is active, a saved password is encrypted with AES-GCM using a key managed by Android Keystore; related values are stored in app-private SharedPreferences. The username may be stored without additional application-level encryption.

Android WebView can also retain authentication cookies and website storage. Turning off password remembering does not, by itself, guarantee that every existing website session or browser storage entry has been removed.

### 5.3 Chrome Browser Extension

The Chrome extension works with an existing signed-in university webpage and its browser-managed session. The reviewed extension code did not show a separate mechanism for collecting or storing university account passwords.

University website storage, browser cookies, and authentication behavior remain subject to the browser and the university website.

## 6. Local Data Storage

The App may store information locally to support features, session restoration, and performance. Storage mechanisms differ by platform.

### 6.1 iOS and iPadOS

Information may be held in Keychain, UserDefaults, app cache and support directories, temporary files, memory, and WKWebView website storage. Some cached content may include university profile, academic, financial, or immigration-related fields.

Although platform protections apply, not every cached record or image is separately encrypted by the App.

### 6.2 Android

Information may be retained in SharedPreferences, Android Keystore-related credential storage, WebView cookies, and other WebView storage. Some profile and other university data may be stored in application-private storage without an additional layer of app-level encryption.

System backup or device migration settings may affect copies of app data. The exact backup behavior depends on the device and operating-system configuration.

### 6.3 Chrome Extension

The extension may store interface preferences and publicly available examination data in Chrome extension storage. Message or course information can remain in active page or extension memory while features are in use, and may not disappear immediately when an individual panel is hidden.

The university website’s browser storage is separate from the extension’s own storage and is not fully controlled by the extension.

## 7. University Servers and Supporting Services

### 7.1 University SARRA2 System

The App connects to the university’s SARRA2 pages and services to provide academic and campus-related features. Normal login, profile, and message requests identified in the audit are directed to the university service, rather than through the App’s configuration Worker.

The App does not control APIU’s data retention, account records, infrastructure, downstream service providers, or authentication-session policies. Consult the university’s official notices for those practices.

### 7.2 Application Configuration and Examination Services

Cloudflare-hosted infrastructure, including Workers, KV, and Durable Objects, supports distribution of app configuration, announcements, version information, and examination schedules.

The reviewed code did **not** show a developer-run student academic-record database or an ordinary route for sending users’ grades, personal profiles, or messages to that configuration service. Individual examination matching may be performed on the device by combining locally available course data with a public examination schedule.

Even when only public information is requested, the service or its infrastructure may process ordinary connection metadata. Hosting-level logs, retention periods, and locations require confirmation from the actual deployed service configuration and provider practices.

The administration interface uses separate administrator authentication data; it is not the same as student SARRA2 login.

### 7.3 External Links and User-Directed Sharing

If you open an outside website, export a file, or share data with another app or service, the destination may receive information you choose to send and may process it under its own privacy policy. The App does not control those destinations after the information has been transferred.

## 8. Optional Translation Services

Some iOS versions offer optional message translation using an operating-system translation framework or remote translation providers. Available remote options may include OpenAI-compatible services and other AI or translation services, including user-configured endpoints.

When you choose a **remote** translation option, the App may send the selected message content, prompts or instructions, requested language, model parameters, and relevant authentication information to that provider. Some translation paths may also transmit technical information, such as operating-system details and temporary identifiers.

**The selected message text is not automatically anonymized before submission to a remote translation provider.** It may include personal information about you or another person.

The handling, retention, potential training uses, subprocessors, and geographic processing of data by remote providers depend on their own policies and arrangements. The App cannot guarantee that a remote provider immediately deletes submitted content or never uses it for other purposes.

Translation output may be cached temporarily in app memory. Removing a local API key or translation cache does not remove information already received by a remote provider. Use caution when translating confidential or sensitive material.

## 9. Device Permissions and System Features

Permissions vary by platform and feature.

### 9.1 Camera and QR Scanning

On supported iOS devices, camera permission may be requested when you start QR-code scanning. The reviewed app code did not show a dedicated function for uploading scanning video frames. Opening a scanned link, after confirmation, may send an ordinary network request to that destination.

### 9.2 Calendar

On supported iOS devices, calendar access may be requested to add examination events and check for previously created entries. The reviewed implementation may request full calendar access rather than write-only access.

Events stored in your system calendar may be synchronized by your chosen calendar provider. Signing out of the App does not remove events already saved there.

### 9.3 Notifications

On supported iOS devices, the App may request notification permission for local message-related notifications. A notification may contain details such as a title or sender. Whether such details appear on a lock screen depends on device settings.

### 9.4 Files, Photos, and Sharing

The App may let you save or export images, PDFs, and other documents through device-provided sharing or file interfaces. Copies managed by external applications or storage services are not automatically removed by the App.

The reviewed Android app has a different set of declared permissions and should not be assumed to implement every iOS feature.

## 10. Cookies, Diagnostics, and Local Usage Information

Cookies and other website data may support SARRA2 sessions through WKWebView, Android WebView, or the desktop browser.

The App may also maintain local diagnostic records. On iOS, diagnostics can include request metadata; a user-initiated diagnostic export can additionally contain certain identifiers or visible page content. On Android, request records may include URL paths and query parameters, which could contain personal or sensitive data.

**A diagnostic export should not be assumed to be anonymous.** Review it before copying or sending it to anyone.

On iOS, Settings > Feedback & Logs > Log Upload Settings provides upload controls without displaying the technical event history. Automatic error reporting is off by default and starts only after you confirm enabling it. You can turn it off and clear queued reports in Settings. Reports sent to the developer-operated support service at config.719100.xyz contain only fixed error and operation categories, app page categories, timestamps, button-press events, request-method categories, numeric status codes and elapsed milliseconds, app/build version, iOS version, and phone/tablet category. They do not include account names, student IDs, passwords, verification or recovery codes, cookies, authentication tokens, request bodies, URLs, document contents, or visible page text. No persistent device or installation identifier is attached. This restricted report is different from the fuller developer-tool export described above.

Structured diagnostic reports also include fixed control and operation-stage names, app-owned source categories, failure categories, numeric HTTP and operating-system error codes, retry counts, response-format categories and item counts, network-type categories (such as Wi-Fi, cellular or offline), foreground/background state, whether saved data is available, and the configuration version. Random launch, workflow, request and upload-bundle references connect related records; these are not persistent device identifiers or university-account identifiers. Network names, IP addresses, full URLs, headers, request or response bodies, raw error descriptions and school-page content are not included in this report schema. Ordinary hosting connection metadata is handled separately as explained below.

Automatic reporting requires renewed confirmation before this expanded schema is enabled, including for users who previously enabled the older reporting format. An automatic report includes a bounded window before and shortly after a detected failure, including related retries; expected user cancellations are not automatically reported as failures. A manual upload sends retained operation records in numbered batches, with a recent failure window first when available. Operation names identify fixed app controls, not values typed or selected by the user. These records are for diagnosing faults, not advertising, user profiling or engagement analytics.

Local operation logs are kept until you explicitly use Settings > Clear Cache > Clear Cache & Logs. Opening pages, switching accounts, restarting the App, successful upload and the age or number of records do not automatically clear this archive. Only a bounded recent window is held in memory; manual uploads read the archive in small batches. Pending automatic-upload envelopes are limited in number and can expire after seven days, but this does not delete their archived operation records. Uninstallation, operating-system actions, unavailable storage or device failure can affect local files. Server reports are limited to the latest 300 and expire after fourteen days; authorized administrators can inspect, download, and delete them. A rotating, salted network hash is used separately for hourly abuse prevention and is not attached to reports. Cloudflare infrastructure necessarily receives network metadata, including the source IP address, and may keep its own operational records. Clearing local records does not delete reports already received by the support service. The App does not include a third-party advertising SDK. Local usage counts and interface preferences may still be kept on the device.

### Voluntary User Feedback

Settings > Feedback & Logs > Send Feedback lets you voluntarily submit a bug report, feature request or suggestion without a GitHub account. The support service at config.719100.xyz receives only the text you enter, its feedback category, a submission reference, the submission time, app/build and operating-system versions, and phone/tablet category. No account credentials, school-page contents or diagnostic logs are attached automatically. You must review the text and confirm removing private information before sending it. Do not include names, student IDs, phone numbers, passwords, verification codes, cookies, tokens or other unnecessary personal information.

Feedback is used for support and product improvements. Authorized administrators review it and may forward approved text to the private SARRA2-Feedback GitHub issue tracker. GitHub processes forwarded information as a separate service. Sending feedback does not automatically publish an Issue. Server feedback shares the bounded report store and is retained for up to fourteen days; administrators may delete it earlier. Forwarded GitHub Issues can be retained longer. Deleting a server report does not delete a GitHub Issue, and closing an Issue does not delete its content. Local drafts and retries remain in memory, are not uploaded automatically, and are discarded when the feedback page is closed. Infrastructure receives ordinary request metadata; a daily-salted network hash is used separately for rate limiting and is not attached to feedback.

## 11. Data Retention and Deletion

There is no single fixed retention period in the reviewed implementation for all personal information cached locally. Different data types and platforms have different deletion behavior.

### 11.1 iOS and iPadOS Sign-Out

Signing out attempts to end the university session and removes certain primary Keychain credentials, authentication cookies, and cached records for the current account.

It does **not** necessarily remove every saved account, account avatar, translation API key, preference, notification record, website-data entry, temporary export, or event already added to a system calendar. A local sign-out also does not prove that the university has revoked every server-side session.

Separate options may be available to remove saved accounts, clear certain caches, or manage translation keys.

### 11.2 Android Sign-Out

Signing out removes selected saved credentials and native cache entries and requests WebView cookie removal. It may leave other WebView data, diagnostics, history, or information still held by active views. The reviewed code does not confirm that this action always revokes the university session on its server.

### 11.3 Chrome Extension and Browser Data

The extension depends on an existing browser session. Closing or hiding an extension panel does not necessarily clear every in-memory result or university website storage entry. Browser or website cleanup may be needed separately.

### 11.4 External Copies and Uninstallation

Files exported to another app, calendar events, cloud-synchronized content, third-party translation submissions, university records, and service-provider logs are not removed by clearing the App’s local cache.

Uninstalling the App may remove some device data, but complete deletion of Keychain items, backups, exported files, or external-system records cannot be guaranteed from the reviewed source code.

## 12. Information Security

The App uses security mechanisms including Apple Keychain, Android Keystore-based password encryption, and HTTPS for its normal university and configuration endpoints.

Protections differ among platforms and features. Some locally cached records lack additional app-level encryption, and certain user-configured local translation services may use HTTP connections. No electronic storage or transmission method is completely risk-free.

Protect access to your device, review saved-login settings, and avoid sending credentials, sensitive diagnostics, or confidential documents to untrusted parties.

## 13. Your Privacy Choices and Rights

Subject to applicable law and the circumstances of the processing, you may have rights to request access to, correction of, deletion of, or restrictions on certain personal information; to object to certain processing; to withdraw consent where consent is the applicable basis; or to exercise other statutory rights.

Available app controls may let you manage saved accounts, caches, translation settings, and device permissions. Their scope differs between platforms, and they do not amount to a guaranteed universal data-erasure function.

The developer can only act on data within the developer’s possession or control. Requests involving official university records or university-managed accounts should be addressed to APIU through its official channels. For information held by independent translation or other external service providers, you may need to contact those providers.

For privacy questions about the App itself, use the contact channel listed in Section 17.

## 14. International Data Processing

University infrastructure, Cloudflare-hosted services, optional translation providers, and operating-system services may process network requests or information in different countries.

Specific geographic locations, retention schedules, subprocessors, and international transfer arrangements could not all be determined from the reviewed source code. Where cross-border processing is subject to legal requirements, the relevant responsible parties must assess and meet those requirements.

Please review the terms and privacy notices of any optional external service before submitting sensitive information to it.

## 15. Independent Application and Academic Information

SARRA2 App is independently developed by a third party and is **not an official APIU application**.

References to APIU, SARRA2, and associated university services identify the systems with which the App interacts. They do not establish that the App is operated by the university.

The App does not control the accuracy, availability, or timing of university-maintained information. Examination schedules, attendance, grades, announcements, and other important records should be verified through official university channels.

## 16. Changes to This Privacy Policy

This Privacy Policy may change when the App’s features, data practices, integrations, or applicable requirements change. Updated versions will identify a revised effective or last-updated date.

Where required by applicable law, additional notice or consent will be sought before materially different processing occurs. Users are encouraged to review the current policy periodically.

## 17. Contact and Privacy Inquiries

For questions about this Privacy Policy, the App’s handling of information, or a privacy-related request, the following identifies the application:

**Application:** SARRA2 App  
**Developer:** Independent Third-Party Developer  

Do not include your university password, authentication tokens, or unnecessary sensitive information in a privacy inquiry.

For questions about the official SARRA2 system or university-maintained student records, contact APIU through its official channels.
