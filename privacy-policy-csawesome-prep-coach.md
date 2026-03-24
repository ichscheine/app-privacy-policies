# CSAwesome Prep Coach Privacy Policy

Last updated: 2026-03-24

CSAwesome Prep Coach is a Chrome extension that adds a study coach panel to CSAwesome on Runestone so a student can follow a daily AP CSA roadmap, open the correct topic, and track mastery locally in the browser.

## Extension Permissions

CSAwesome Prep Coach declares the following Chrome permission:

- `storage`

The extension runs on the following site pattern through its content script matches:

- `https://runestone.academy/ns/books/published/csawesome2/*`

`storage` is used only to save roadmap progress, checklist completion, streaks, achievements, auto-advance preference, and interface state on the user's device.

## What The Extension Stores

- roadmap progress and mastered blocks
- checklist completion state for the current study block
- streaks, milestone badges, and related progress markers
- user interface state such as selected view and collapse state
- settings such as whether auto-advance is enabled

## How Data Is Used

The extension uses this data only to:

- show the current AP CSA study plan
- remember completed work across sessions
- reopen the correct CSAwesome target
- preserve the student's local coach preferences

The extension reads the visible CSAwesome table of contents already present on the current Runestone page so it can open the matching topic for the current roadmap block.

## Where Data Goes

CSAwesome Prep Coach stores its progress and preference data locally using Chrome extension storage on the user's device.

Based on the current extension repo, this data is not transmitted to external application servers and is not shared with third parties.

## Host Access

The extension runs only on CSAwesome pages hosted on Runestone that match its manifest:

- `https://runestone.academy/ns/books/published/csawesome2/*`

It is not designed to read browsing history outside the active supported CSAwesome page.

## Third-Party Sharing And Remote Code

The current extension does not sell, transfer, or share user data with third parties.

The extension packages its code locally and does not execute remotely hosted code based on the current project files.

## Chrome Web Store Disclosure Summary

- website content is accessed: yes, only on supported CSAwesome pages needed for navigation
- webpage content is transmitted for analysis: no
- user activity within the extension is stored: yes, local study progress and preferences only
- data is stored on the device: yes
- data is sold to third parties: no
- data is used for advertising or marketing: no
- data is used for creditworthiness or other eligibility determinations: no
- data is sent to a third-party remote service by default: no

## User Controls

You can remove saved progress and preferences by clearing the extension's storage or uninstalling the extension.

## Changes To This Policy

If the extension's permissions, host access, or data practices change in a future release, this policy should be updated before that version is distributed.
