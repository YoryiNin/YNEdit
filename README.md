# YNEdit - Support and Legal

This repository hosts the support and legal pages for **YNEdit**, an Android video editor by **YNStudios**.

- **Privacy Policy:** [English](privacy-en.html) / [Español](privacy-es.html)
- **Terms of Use:** [English](terms-en.html) / [Español](terms-es.html)
- **AdMob verification:** [app-ads.txt](app-ads.txt)
- **Support and privacy contact:** [yntoxicboythegamer@gmail.com](mailto:yntoxicboythegamer@gmail.com)

## Analytics disclosure

Firebase Analytics is integrated. The app records project creation, coarse media-import category, selected editor tools, playback starts, recording starts, clip splits/reversals, Premium feature status changes, and export start/completion/failure. Firebase also collects its standard app/device analytics and may infer approximate country or region from IP address; the app does not request precise location. Do not add event parameters containing media, project identifiers or names, file paths, edited text, or user content.

Before release, configure consent or opt-out where required in target regions (the app currently has no in-app Analytics opt-out), verify Firebase data-processing and retention settings, complete Google Play Data safety answers, and confirm the deployed event list matches this disclosure.

The app uses Google test AdMob identifiers by default. Configure production values in Gradle properties before release: `yneditAdMobAppId`, `yneditRewardedAdUnitId`, and `yneditBannerAdUnitId`. The IDs must belong to the same AdMob publisher/app. Google User Messaging Platform (UMP) requests consent before initializing Mobile Ads and exposes privacy options in Settings when required; configure and test the applicable consent messages in AdMob Privacy & messaging before release. Ads are not requested unless UMP permits them. After four active projects, a completed rewarded ad unlocks each further project. The two Premium subscription product IDs default to `ynedit_premium_monthly` and `ynedit_premium_annual`; configure `yneditMonthlySubscriptionId` and `yneditAnnualSubscriptionId` to exactly match the subscription product IDs created in Play Console. Prices are loaded from Google Play and are not hardcoded. Google Play Billing checks owned subscriptions on connection and when the app resumes; active subscriptions remove all ads and the project limit, and the entitlement is removed when Play no longer reports an active purchase. Play handles automatic renewal, expiry, cancellation, and refunds. No purchase token is sent to Firebase Analytics.

Before release, create and activate the monthly and annual subscription products in Play Console, configure production AdMob IDs and consent handling for the target regions, then test purchase, renewal, cancellation, restore, expiry, and ad removal using Play internal testing. Client-side billing is used; add server-side purchase-token verification if stronger entitlement protection is required.

These pages are a project-specific draft and are not legal advice. Have the final terms, privacy notice, and store disclosures reviewed for the regions where the app will be distributed.
