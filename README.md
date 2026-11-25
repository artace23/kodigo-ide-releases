Kodigo IDE: Downloads
Pagsulat ng Kodigo, Sa Sariling Wika.

This repository holds the Windows installers and release notes for Kodigo IDE, a desktop code editor for Windows that opens in Filipino. It is built on Code - OSS, keeps the VS Code extension model, and adds local tools (X-Ray, Impact, Flow, Memory, Replay) that read your project without sending it anywhere.

Kodigo has no built-in AI. AI assistants such as Claude Code and Codex are separate extensions you choose to install.

Download
Open the latest release.
Download Kodigo-IDE-Setup-<version>.exe.
Run it. It installs for your user account only and does not need administrator rights.
Requirements: Windows 10 or 11, 64-bit.

Check the download
Each release lists the SHA-256 of its installer. To compare it, run this in PowerShell from the folder with the file:

Get-FileHash .\Kodigo-IDE-Setup-<version>.exe -Algorithm SHA256
The value must match the one in the release notes exactly. If it doesn't, don't run the file.

Windows may show a warning
The installer is not yet code-signed, so Windows SmartScreen may say it doesn't recognize the app. This is expected until a signing certificate is in place. Check the SHA-256 above before choosing to run it.

Updates
Kodigo checks this repository once a day, at startup, for a newer release and tells you if there is one. It never downloads or installs anything by itself. You can turn the check off with the setting kodigo.updates.checkOnStartup, or run Kodigo: Check for Updates any time. The only request is to the GitHub API for this repository's latest release, with no project or personal data.

Privacy
No telemetry and no crash upload. The Kodigo tools run locally. The editor reaches the internet only when you search or install extensions (Open VSX) or check for updates (GitHub).

Claude Code and Codex
Kodigo can install the official Claude Code (Anthropic) and Codex (OpenAI) extensions from Open VSX after you agree. They are not included in the installer, because their licenses don't allow redistribution. You sign in inside each extension with your own account.

Credits and licenses
Kodigo IDE is based on Code - OSS, Copyright (c) Microsoft Corporation, licensed under the MIT License. Electron, Chromium and other components keep their own licenses. Their full notices ship inside the application. Kodigo IDE is not affiliated with or endorsed by Microsoft.

Reporting problems
Use this repository's Issues. Please include your Kodigo version (Help > About) and Windows version. Don't paste passwords, keys or private code.

