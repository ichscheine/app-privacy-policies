# CWS Autofill Privacy Policy

Last updated: 2026-03-24

CWS Autofill is a Chrome extension that helps a developer turn a local `privacy-policy.md` file into copy-ready Chrome Web Store listing and privacy-form answers.

## Extension Permissions

CWS Autofill declares these Chrome permissions:

- `storage`
- `sidePanel`

CWS Autofill does not declare any host permissions. These permissions are used only to keep the extension side panel available and save the generated profile, listing fields, permission justifications, and checklist state so the developer can continue the same workflow across sessions.

## Data Categories CWS Autofill Handles

When you use CWS Autofill, the extension may access or store:

- the local `privacy-policy.md` file content that you explicitly choose to upload
- generated Chrome Web Store field values derived from that file
- saved extension state such as the current profile, generated field values, permission justifications, and publish checklist state

CWS Autofill does not request or intentionally collect:

- website content from arbitrary pages
- browsing history
- precise location
- contacts
- financial account or payment card data
- authentication credentials
- analytics identifiers

## How CWS Autofill Uses Data

CWS Autofill uses accessed data only to:

- parse the uploaded privacy-policy markdown locally in the browser
- generate copy-ready Chrome Web Store listing and privacy answers and justifications
- render the popup and side panel UI so the developer can review and copy the generated values
- save the current profile locally so the developer does not need to regenerate it every time

CWS Autofill is not designed to:

- sell personal information
- serve ads
- build advertising profiles
- make credit, lending, employment, housing, insurance, or similar eligibility decisions

## Where Data Goes

CWS Autofill processes the uploaded markdown locally inside the extension. It does not send the uploaded file, generated outputs, or saved profile data to external application servers.

If Chrome sync storage is available for the user's browser profile, saved extension state may be stored through Chrome's sync mechanism. Otherwise, the extension uses local extension storage on the device.

## Third-Party Services

CWS Autofill does not use ad networks, analytics SDKs, social media trackers, or external AI or model providers. It does not rely on remotely hosted code.

## Data Storage And Retention

CWS Autofill stores the current profile, generated listing and privacy answers, permission justifications, and related settings in `chrome.storage.sync` when available, or `chrome.storage.local` as a fallback.

That saved state remains until the user clears extension storage, removes the extension, or clears the associated browser profile data.

## Chrome Web Store Disclosure Summary

- website content is accessed: no
- webpage content is transmitted for analysis: no
- user activity within the extension is stored: yes, saved profile values and generated form text only
- data is stored on the device: yes
- data is sold to third parties: no
- data is used for advertising or marketing: no
- data is used for creditworthiness or other eligibility determinations: no
- data is sent to a third-party remote service by default: no

`sidePanel` is a Chrome permission, not a standalone data category. The main data this extension handles is the user-provided markdown content and the generated profile values stored locally to support the requested workflow.

## User Controls

You control whether to upload a local `privacy-policy.md` file and whether to keep the generated profile in extension storage. You can remove saved data by clearing the extension's storage or uninstalling the extension.

## Changes To This Policy

If CWS Autofill changes its permissions, storage behavior, or data flow, this policy should be updated before publication or release.
