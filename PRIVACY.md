---
layout: default
title: Privacy Policy – Seam
---
# Privacy Policy

**Effective date:** June 15, 2026
**Last updated:** June 15, 2026

This Privacy Policy describes how Seam ("we," "us," or "the app") handles information when you use our iOS app.

## TL;DR

Seam stores everything you save on your own device and in your own iCloud account. We don't run a server, we don't collect your data, we don't have analytics, we don't share anything with anyone, and there are no ads. The only network requests the app makes are to the product pages you choose to save — and the results stay on your device.

## What we collect

**Nothing on a server we control.** We do not operate any backend database, analytics service, advertising network, or tracking system. Seam does not have a developer-side account system or login.

The app does store information **on your device** and synchronizes it to **your private iCloud database** so it's available across your other Apple devices signed in to the same Apple ID. This data is encrypted in transit and at rest by Apple, and we have no access to it. This includes:

- Product items you choose to save (brand, item name, price, source URL, image URL, product image, category, notes, saved date)
- Your profile name and profile photo (if you set one)
- App preferences (view mode, sort option, onboarding state)

We never see, access, or transmit this data outside of your own iCloud account.

## How web scraping works

When you share a product URL to Seam, the app fetches that URL using a standard `URLSession` request and, if needed, a hidden `WKWebView` instance — both of which behave like a normal mobile Safari browser. The app extracts the product's brand, name, price, and image from the publicly-available HTML, JSON-LD metadata, and Open Graph meta tags of the page.

This activity happens entirely on your device. No URLs or scraped content are sent to us or to any third party. Retailers see the request as if you were visiting their page from Safari, which you would have done anyway by tapping the share button.

## First-launch homepage pre-load

On first launch, Seam silently loads the homepages of approximately six common retail websites (COS, SSENSE, H&M, Aritzia, Nordstrom, Farfetch) to warm up the in-app browser's cookie store. This makes future scrapes more reliable on websites that use bot-protection systems. This loading happens once, ever, after onboarding completes. Approximately 5 megabytes of data is transferred over WiFi or your cellular connection. No data is sent to us as part of this process — the requests go directly from your device to the retailers' servers.

## Affiliate links

When you tap the "View item" button to open one of your saved products in your browser, Seam may route you through Skimlinks, a third-party affiliate marketing service. Skimlinks rewrites the destination URL to include affiliate tracking parameters before redirecting you to the retailer.

If you then make a purchase on that retailer's site, Seam earns a small commission paid by the retailer. The commission **does not change the price** you pay and does **not** influence which items are saved, suggested, or displayed in the app.

Skimlinks may set cookies on the destination retailer's site in your browser as part of this redirect. Their own privacy policy is available at <https://skimlinks.com/privacy-policy>.

You can avoid the redirect entirely by copying the source URL from the item details and opening it directly in your browser — Seam works exactly the same either way.

We disclose this in compliance with FTC and EU advertising disclosure rules.

## iCloud sync (CloudKit)

Seam uses Apple's CloudKit framework to sync your saved items between your Apple devices. Your data is stored in your **private** CloudKit database, which only you can access. We — the developer — cannot view, export, or modify your private CloudKit data. Apple's privacy documentation for CloudKit applies in full.

If you sign out of iCloud, disable iCloud Drive for Seam, or are signed in with a different Apple ID, sync will pause. Your local data on the device remains accessible.

## What we don't do

- We do not display advertisements
- We do not include third-party analytics SDKs (Mixpanel, Amplitude, Firebase Analytics, etc.)
- We do not include third-party tracking or attribution SDKs
- We do not request the App Tracking Transparency permission
- We do not collect device identifiers (IDFA, IDFV) or location
- We do not collect contact info, health data, financial info, or any other category requiring consent under iOS privacy rules
- We do not sell, rent, share, or otherwise transfer your data to anyone, for any reason

## Children's privacy

Seam is rated 4+ in the App Store and is suitable for all ages. We do not knowingly collect data from anyone, including children under the age of 13 (or 16 in the European Union). Because Seam does not collect any personal data on a server we control, COPPA and GDPR-Kids compliance issues do not arise.

## Your rights

Because all of your data lives on your device and in your private iCloud:

- **To export your data**: open any item, copy the text you want, or use iOS's standard backup/restore features
- **To delete your data**: use the "Clear all items" button in the app, or simply uninstall the app and remove its iCloud data via Settings → Apple ID → iCloud → Manage Account Storage → Seam
- **To request access, deletion, correction, or portability under GDPR / CCPA / CCRA**: not applicable, as we do not hold any of your data on our systems. We have nothing to deliver, delete, or correct. Direct any such requests to Apple, as your iCloud data is stored on their infrastructure.

## Changes to this policy

We may update this policy from time to time. If we make material changes — for example, adding analytics or a backend service — we will update the "Last updated" date at the top and provide notice within the app before the change takes effect. Continued use of the app after a material change indicates acceptance of the updated policy.

## Contact

If you have questions about this policy or about Seam, email us at:

**hello@seamapp.io**

For Apple-related issues (App Store, billing, parental controls, iCloud), please contact Apple directly.

---

_This policy is provided in plain English to be readable. It is not legal advice. If your use of Seam is regulated in a jurisdiction with specific requirements (e.g., HIPAA, COPPA processing as a "covered entity," etc.), you are responsible for ensuring your use complies. We are happy to clarify the technical facts above to assist your compliance assessment._
