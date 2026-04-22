# Picamy Hosted Privacy Policy

Last updated: 2026-04-22

Picamy Hosted is a Chrome extension for rental hosts. It analyzes the active listing page on supported rental platforms, currently Airbnb and VRBO, identifies photo issues that may reduce click intent or booking performance, and returns ranked visual recommendations through a hosted API.

Public privacy policy URL for Chrome Web Store submissions:
`https://github.com/ichscheine/air-visual-privacy/blob/main/privacy-policy.md`

Support contact:
`amy@steamify.me`

## What Picamy Hosted does

When a host opens Picamy Hosted on a supported rental-platform listing page, currently Airbnb or VRBO, the extension may:

- read visible listing content from the active supported listing page
- detect listing image URLs and basic image metadata
- send selected listing context to Picamy's hosted API
- receive ranked photo recommendations and preview guidance
- store local recommendation decisions and access settings on the device
- accept waitlist requests from hosts who request access inside the extension

Picamy Hosted is built for a narrow, user-facing purpose: improving rental-listing photo presentation for hosts on supported marketplaces.

## Extension Permissions

Chrome permissions:

- `activeTab`
- `sidePanel`
- `scripting`
- `storage`
- `tabs`

Host permissions:

- `https://www.airbnb.com/*`
- `https://*.airbnb.com/*`
- `https://www.vrbo.com/*`
- `https://*.vrbo.com/*`
- `https://air-visual-api-147870447783.us-central1.run.app/*`
- `https://airvisual.steamify.me/*`

Why these permissions are used:

- `activeTab`, `tabs`, and supported host permissions let Picamy read the current supported rental-platform listing page the host is actively viewing
- `scripting` allows the content script to run or re-run on supported rental-platform pages
- `sidePanel` displays the Picamy analysis experience
- `storage` stores invite-code access, waitlist email, local recommendation decisions, and an installation identifier
- the hosted API permission allows the extension to call Picamy's backend

Chrome extension permissions:

- `activeTab`
- `sidePanel`
- `scripting`
- `storage`
- `tabs`

host permissions:

- `https://www.airbnb.com/*`
- `https://*.airbnb.com/*`
- `https://www.vrbo.com/*`
- `https://*.vrbo.com/*`
- `https://air-visual-api-147870447783.us-central1.run.app/*`
- `https://airvisual.steamify.me/*`

### Permission justification

`activeTab`

- Used only to access the active supported rental-platform tab when the host opens Picamy on that page.

`sidePanel`

- Used only to present the Picamy recommendation interface inside Chrome's side panel.

`scripting`

- Used only to inject or re-inject the packaged content script on supported rental-platform pages so listing context can be extracted.

`storage`

- Used only to store invite-code access, waitlist email, recommendation decisions, and an installation identifier required for core product behavior.

`tabs`

- Used only to identify the current active supported rental-platform tab and route extraction or side-panel actions to that tab.

`https://www.airbnb.com/*`, `https://*.airbnb.com/*`, `https://www.vrbo.com/*`, and `https://*.vrbo.com/*`

- Used only to read the currently open supported listing page and its visible listing context when the host actively invokes Picamy.

`https://air-visual-api-147870447783.us-central1.run.app/*`

- Used only to send listing context to Picamy's hosted API and receive recommendation results.

`https://airvisual.steamify.me/*`

- Used only as an alternate Picamy API origin so the extension can continue reaching the hosted service if the primary API hostname is unavailable.

## Data Picamy handles

Picamy may access, transmit, or store these categories of data:

### Website content

From the active supported listing page only, Picamy may read:

- current page URL
- listing title
- visible page text
- nightly-rate text when visible
- occupancy hints when visible
- amenity terms visible on the page
- image URLs
- image alt text
- basic image metadata such as dimensions

Picamy is not designed to read browsing history outside the active supported listing page being analyzed.

### User-submitted contact or listing details

If a host requests access from inside the extension, Picamy may collect:

- email address
- listing URL from a supported rental platform

### User activity

Picamy may record product activity such as:

- recommendation marked for update
- recommendation skipped
- analysis completed
- invite request submitted

### Local extension storage

Picamy stores some data locally on the device:

- saved invite code
- saved waitlist email
- saved recommendation decisions
- installation identifier used for product analytics

## Data Picamy does not intentionally collect

Picamy does not request or intentionally collect:

- precise location
- contacts
- health information
- payment card or financial account information
- personal communications
- authentication credentials other than the invite code entered for Picamy access
- browsing history outside the active supported listing page

## How data is used

Picamy uses data only to:

- identify the current supported listing
- analyze the listing's visible photo context
- generate ranking, edit, and sequencing recommendations
- deliver preview guidance inside the extension
- remember host decisions locally
- manage invite-only access
- collect waitlist requests
- measure product behavior for future product improvement and experimentation

Picamy is not designed to:

- sell personal information
- serve ads
- build advertising profiles
- run cross-site tracking
- make credit, lending, employment, housing, insurance, or similar eligibility decisions

## Where data goes

### Picamy hosted API

By default, selected listing context and image references are sent from the extension to Picamy's hosted API:

`https://air-visual-api-147870447783.us-central1.run.app`

The extension may also use this alternate API origin for the same hosted service:

`https://airvisual.steamify.me`

That API:

- validates invite-only access
- fetches listing image URLs transiently from supported rental platforms and related CDNs
- prepares the model request
- returns structured recommendations to the extension
- accepts waitlist requests
- records selected product events

Picamy is designed for transient analysis. The extension does not intentionally persist the full extracted listing payload in extension storage, and the hosted API is not intended to maintain a user-facing database of full listing payloads.

### Google Gemini Developer API

Picamy's hosted API sends selected listing context and image data to the Google Gemini Developer API so the model can analyze listing photos and return recommendations.

### Supabase

Picamy uses Supabase for:

- waitlist requests
- invite operations support
- product event tracking

### Resend

If invite-request email notifications are enabled, Picamy uses Resend to:

- notify the owner about new invite requests
- deliver approved invite codes to hosts by email

### Listing image hosts

Picamy's hosted API may fetch listing images from Airbnb-controlled or VRBO-controlled hosts and related CDN URLs when preparing analysis. If additional rental platforms are supported later, the same pattern applies to those platforms' listing-image hosts.

## Third-party services

Picamy may send data to:

- Picamy's hosted API
- Google Gemini Developer API
- Resend for transactional invite emails when enabled
- Supabase
- supported rental-platform pages and listing-image hosts as needed for analysis

Picamy does not include:

- ad networks
- advertising SDKs
- social media trackers
- data broker integrations

## Remote code

Picamy does not load or execute remotely hosted code. The extension code shipped to Chrome is packaged inside the extension bundle. The hosted API returns data only; it does not provide executable code to the extension.

## Storage and retention

Locally on device:

- invite code, waitlist email, installation ID, and recommendation decisions may remain until the host clears extension storage or removes the extension

Remotely:

- waitlist requests and product events may be stored in Supabase for operational follow-up and product analysis
- invite-request notification emails and approved invite-code emails may be processed by Resend when email delivery is enabled
- Picamy's hosted API is intended for transient analysis rather than durable storage of full extracted listing payloads

## Chrome Web Store dashboard mapping

This section is written to align with the Chrome Web Store listing and privacy-form disclosures.

### Data categories to disclose as handled

- Website content: yes
- Personal information submitted by the user: yes, email address and listing URL when requesting access
- User activity: yes, recommendation decisions and related product events
- Local device storage: yes
- Remote data transmission: yes

### Data categories not handled or not intentionally collected

- Precise location: no
- Health information: no
- Financial or payment information: no
- Personal communications: no
- Browsing history outside the active supported listing page: no
- Contacts: no

### Data handling answers

- Data is used to provide the extension's core photo-analysis and recommendation feature: yes
- Data is used for invite-only access and waitlist operations: yes
- Data is used for internal product analytics and improvement: yes
- Data is sold to third parties: no
- Data is used for advertising or marketing: no
- Data is used for creditworthiness or eligibility decisions: no

## Suggested Chrome Web Store form answers

Use the following wording when filling the Chrome Web Store privacy and data-use form for Picamy Hosted:

- Website content: `Yes` — collected and transmitted to analyze the active supported rental listing page.
- Personal information: `Yes` — email address and listing URL, only when the user requests access from inside the extension.
- User activity: `Yes` — recommendation decisions and related product events inside the extension.
- Location: `No`
- Financial and payment information: `No`
- Health information: `No`
- Personal communications: `No`
- Web history: `No` — Picamy does not read browsing history outside the active supported listing page.
- Contacts: `No`
- Data sold to third parties: `No`
- Used for advertising or marketing: `No`
- Used for creditworthiness or eligibility decisions: `No`
- Primary purpose: analyze rental-listing photos and return host-facing optimization recommendations.
- Secondary operational purpose: manage invite-only access, waitlist requests, and service reliability.

## Chrome Web Store Disclosure Summary

For Chrome Web Store disclosure purposes, Picamy's behavior can be summarized as follows:

- website content is accessed: yes
- personal identifiers submitted by the user are collected: yes, email address and listing URL when requesting access
- webpage content is transmitted for analysis: yes
- user activity within the extension is stored: yes, recommendation decisions and related product events
- local device storage is used: yes
- data is sent to a remote service by default: yes
- data is sold to third parties: no
- data is used for advertising or marketing: no
- data is used for creditworthiness or other eligibility determinations: no

## User controls

Hosts control whether to:

- open Picamy on a supported listing page
- request access with email address and listing URL
- save an invite code locally
- keep or clear local extension storage

To remove locally stored data, clear Chrome extension storage for Picamy or uninstall the extension.

## Chrome Web Store Limited Use

Picamy uses and transfers user data only to provide or improve its user-facing short-term-rental photo-analysis feature set. Picamy's use of user data complies with the Chrome Web Store User Data Policy, including the Limited Use requirements.

## Changes to this policy

If Picamy changes its permissions, hosted providers, data flows, or Chrome Web Store disclosures, this policy should be updated before release.
