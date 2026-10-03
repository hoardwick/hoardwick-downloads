# Hoardwick — Downloads

Official download host for **Hoardwick**, a desktop media archiving tool for Windows.

Hoardwick is local-first. It packs its own engine and runtime, so there is nothing else
to install: unzip it, double-click the launcher, and the interface opens in your browser.
Your URLs never leave your machine.

## Download

Get the latest build from the [**Releases**](https://github.com/hoardwick/hoardwick-downloads/releases/latest) page.

| Asset | Notes |
|---|---|
| `Hoardwick-win-x64.zip` | Windows 10 / 11, 64-bit. Portable — no installer, no admin rights. |
| `SHA256SUMS.txt` | SHA-256 checksum for the archive. |

The archive filename is deliberately version-free, so the link above always resolves to
the current build. The exact version is recorded inside the archive (`version.txt`), in
the release title, and on the website.

## Verify before running (recommended)

In PowerShell, in the folder where you saved the archive:

```powershell
certutil -hashfile Hoardwick-win-x64.zip SHA256
```

Compare the result with the matching line in `SHA256SUMS.txt`. They must be identical.

## Requirements

- Windows 10 or Windows 11, 64-bit
- No Python, no Node.js, no separate runtimes — everything needed ships inside the archive
- About 200 MB of free disk space after extraction

## Getting started

1. Unzip `Hoardwick-win-x64.zip` anywhere (for example `D:\Hoardwick`).
2. Double-click **`Start Hoardwick.bat`**.
3. Your browser opens the local interface — paste a URL and start archiving.

Windows SmartScreen may warn about an unrecognised publisher, because the build is not
code-signed. Either choose *More info → Run anyway*, or verify the checksum above first.

## Support

- Email: support@hoardwick.com
- Refund policy: https://hoardwick.com/legal/refund
- Terms of service: https://hoardwick.com/legal/terms
- Third-party licences: https://hoardwick.com/legal/licenses

## About this repository

This repository hosts **release downloads only**. It does not contain the application
source code. Builds are produced from a private repository and published here so that
every release has a permanent, checksum-verifiable download location.

Copyright (c) 2026 Hoardwick. All rights reserved. See [LICENSE](LICENSE).
