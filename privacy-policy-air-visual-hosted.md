# Air Visual Hosted Privacy Policy

Last updated: 2026-03-23

Air Visual Hosted is a Chrome extension for Airbnb hosts. It analyzes the active Airbnb listing page, identifies photo issues that may reduce click intent or booking performance, and returns ranked visual recommendations through a hosted API.

Support contact: `amy@steamify.me`

## What Air Visual Does

When a host opens Air Visual on an Airbnb listing page, the extension may:

- read visible listing content from the active Airbnb page
- detect listing image URLs and basic image metadata
- send selected listing context to Air Visual's hosted API
- receive ranked recommendations and preview guidance
- store local recommendation decisions and access settings on the device
- accept waitlist requests from hosts who request access inside the extension

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
- `https://air-visual-api-147870447783.us-central1.run.app/*`

These permissions are used to access the active Airbnb listing page, present the side panel, run packaged content scripts, store invite and recommendation state, and call Air Visual's hosted backend.

## Data Air Visual Handles

Air Visual may access, transmit, or store these categories of data:

- website content from the active Airbnb page only, including the current page URL, listing title, visible page text, nightly-rate text when visible, occupancy hints when visible, amenity terms visible on the page, image URLs, image alt text, and basic image metadata such as dimensions
- user-submitted contact or listing details, specifically email address and Airbnb listing URL when a host requests access from inside the extension
- user activity such as recommendation marked for update, recommendation skipped, analysis completed, and invite request submitted
- local extension storage including saved invite code, saved waitlist email, saved recommendation decisions, and an installation identifier used for product analytics

Air Visual does not request or intentionally collect:

- precise location
- contacts
- health information
- payment card or financial account information
- personal communications
- browsing history outside the active Airbnb listing page

## How Data Is Used

Air Visual uses data only to:

- identify the current Airbnb listing
- analyze the listing's visible photo context
- generate ranking, edit, and sequencing recommendations
- deliver preview guidance inside the extension
- remember host decisions locally
- manage invite-only access
- collect waitlist requests
- measure product behavior for future product improvement and experimentation

Air Visual is not designed to:

- sell personal information
- serve ads
- build advertising profiles
- run cross-site tracking
- make credit, lending, employment, housing, insurance, or similar eligibility decisions

## Where Data Goes

By default, selected listing context and image references are sent from the extension to Air Visual's hosted API at `https://air-visual-api-147870447783.us-central1.run.app`.

That API:

- validates invite-only access
- fetches Airbnb image URLs transiently
- prepares the model request
- returns structured recommendations to the extension
- accepts waitlist requests
- records selected product events

Air Visual's hosted API sends selected listing context and image data to the Google Gemini Developer API so the model can analyze listing photos and return recommendations.

Air Visual also uses Supabase for:

- waitlist requests
- invite operations support
- product event tracking

Air Visual may fetch listing images from Airbnb-controlled hosts or related CDN URLs when preparing analysis.

## Third-Party Services

Air Visual may send data to:

- Air Visual's hosted API
- the Google Gemini Developer API
- Supabase
- Airbnb-controlled pages and image hosts as needed for listing analysis

Air Visual does not include:

- ad networks
- advertising SDKs
- social media trackers
- data broker integrations

Air Visual does not load or execute remotely hosted code. The hosted API returns data only.

## Storage And Retention

Locally on the device:

- invite code, waitlist email, installation ID, and recommendation decisions may remain until the host clears extension storage or removes the extension

Remotely:

- waitlist requests and product events may be stored in Supabase for operational follow-up and product analysis
- Air Visual's hosted API is intended for transient analysis rather than durable storage of full extracted listing payloads

## Chrome Web Store Dashboard Mapping

- website content: yes
- personal information submitted by the user: yes, email address and Airbnb listing URL when requesting access
- user activity: yes, recommendation decisions and related product events
- local device storage: yes
- remote data transmission: yes
- precise location: no
- health information: no
- financial or payment information: no
- personal communications: no
- browsing history outside the active Airbnb page: no
- contacts: no

## Changes To This Policy

If Air Visual's permissions, supported providers, or data flows change, this policy should be updated before publication or release.
