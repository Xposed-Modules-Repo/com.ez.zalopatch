# Zalo Patch

Zalo Patch is an open-source LSPosed module for customizing Zalo while keeping compatibility
fail-soft and exact-version based.

## Compatibility

- Zalo package: `com.zing.zalo`
- Supported build: Zalo 26.08.02 (`versionCode 260802903`)
- Android 8.0 (API 26) or newer
- LibXposed API 102

Unsupported Zalo artifacts do not use nearest-version symbols. Features requiring unavailable
anchors remain disabled until an exact signed compatibility entry or bundled map exists.

## Features

- Clean up bottom navigation, inbox, chat, and Me-screen surfaces.
- Add inbox category controls for chats, groups, official accounts, and strangers.
- Conservatively filter reviewed promotional notifications.
- Suppress selected analytics and advertising paths.
- Keep an optional local notification history with bounded retention and export.
- Record one-to-one call audio after the user enables the feature.
- Fetch signed exact-artifact compatibility mappings with bundled offline fallback.

## Installation

1. Install the signed APK from this repository's Releases page.
2. Enable Zalo Patch in LSPosed.
3. Scope the module only to Zalo (`com.zing.zalo`).
4. Open Zalo Patch, choose settings, and use the explicit Restart Zalo action to apply them.

Call recording is opt-in. Users are responsible for complying with consent and recording laws.

## Privacy

- Diagnostic reports upload only after explicit user review and action.
- Notification history stays in local app storage until exported or cleared.
- Call recordings are stored on the device.

## Source And Support

- Source: https://github.com/amarinne/zalo-patch
- Issues: https://github.com/amarinne/zalo-patch/issues
- Signed upstream release: https://github.com/amarinne/zalo-patch/releases/tag/v0.4.196

Zalo Patch is unofficial and is not affiliated with or endorsed by Zalo or VNG.
