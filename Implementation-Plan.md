# Rebrand RustDesk to "Digital Solution"

This plan outlines the steps to rebrand the RustDesk application to "Digital Solution" and update the privacy policy and contact details according to your client's requirements.

## User Review Required

> [!WARNING]
> While we are changing the UI branding (name, logo, and about page text) to "Digital Solution", the underlying source code must legally retain its original AGPLv3 license and copyright headers.

## Open Questions

> [!IMPORTANT]
> 1. Do you have a specific URL for the Privacy Policy, or should I just display the text "Privacy Policy: Digital Solutions - Kolkata Apple Authorised Dealer" in the About page?
> 2. For the Logo, do you want me to generate an AI logo (using my image generation tool) and replace the existing RustDesk icons?

## Proposed Changes

### Core Rust Configuration

#### [MODIFY] Cargo.toml
- Update `ProductName` to "Digital Solution"
- Update `FileDescription` to "Digital Solution Remote Desktop"
- Update `OriginalFilename` to "digitalsolution.exe"
- Update `[package.metadata.bundle] name` to "Digital Solution"

### Flutter UI (Settings / About Page)

#### [MODIFY] flutter/lib/desktop/pages/desktop_setting_page.dart
- Update the "About RustDesk" title to "About Digital Solution".
- Remove or update the "rustdesk.com" website links.
- Add the contact and privacy text: "Digital Solutions - Kolkata Apple Authorised Dealer".

#### [MODIFY] flutter/lib/mobile/pages/settings_page.dart
- Update the "About RustDesk" title to "About Digital Solution".
- Remove or update the "rustdesk.com" website links.
- Add the contact and privacy text: "Digital Solutions - Kolkata Apple Authorised Dealer".

### Localization (Translations)

#### [MODIFY] src/lang/en.rs
- Search and replace visible instances of "RustDesk" with "Digital Solution" in the English translations (e.g., "Powered by Digital Solution", "Install Digital Solution", etc.).

### Logo Update

#### [NEW] Assets / Logo
- Generate a new logo image.
- Replace the main icons in `res/` (e.g., `res/32x32.png`, `res/128x128.png`, `res/128x128@2x.png`).

## Verification Plan

### Manual Verification
- We will build the Flutter application (or review the code changes) to ensure that the UI text correctly displays "Digital Solution".
- We will verify that the About page correctly displays the updated privacy policy text and contact name.
