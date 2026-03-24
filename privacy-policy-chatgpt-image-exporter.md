# ChatGPT Image Exporter Privacy Policy

Effective date: 2026-02-26

ChatGPT Image Exporter is a Chrome extension that enables users to bulk-download images from the ChatGPT Images tab (`https://chatgpt.com/images`) directly to their local device.

This extension is designed to operate entirely within the user's browser environment.

It does not collect, store, transmit, sell, or share personal data.

## Data Collection

ChatGPT Image Exporter does not collect:

- personal information
- chat history
- image content
- prompts
- account information
- authentication tokens
- usage analytics
- device information
- browsing history

No data is sent to any external server.

## Local Processing Only

All processing occurs locally in your browser.

The extension:

- accesses the ChatGPT Images page only after user interaction
- fetches image files directly from ChatGPT's domain
- saves images and optional metadata files to your local Downloads folder
- stores export settings locally using Chrome's storage API

No data leaves your machine.

## Permissions Explanation

The extension requests the following permissions solely to fulfill its single purpose:

- `activeTab`: Access the current ChatGPT Images tab after user click.
- `downloads`: Save exported image files locally.
- `storage`: Save export preferences and resume state locally.
- `scripting`: Inject export logic into the ChatGPT Images page.
- `offscreen`: Enable reliable background downloading under Manifest V3.
- host permission for `chatgpt.com`: Access the ChatGPT Images page to retrieve image metadata and download URLs.

These permissions are not used for tracking, advertising, or monitoring activity.

## No Remote Code

ChatGPT Image Exporter does not load or execute remote code.

All JavaScript, HTML, and CSS files are packaged within the extension.

The extension does not connect to external APIs, analytics platforms, or third-party services.

## Data Retention

The extension does not retain personal or image data beyond:

- user-selected export settings stored locally
- resume index stored locally

Users may remove this data at any time by uninstalling the extension or clearing Chrome extension storage.

## Third-Party Services

This extension does not use:

- analytics services
- tracking scripts
- advertising networks
- external databases
- cloud storage

It interacts only with `chatgpt.com` as part of its intended export functionality.

## Changes To This Policy

If material changes are made to this privacy policy, the updated version will be published with a revised effective date.

## Contact

If you have questions regarding this privacy policy, you may contact:

Steamify LLC  
amy@steamify.me
