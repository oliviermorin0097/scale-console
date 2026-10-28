<img src="app-icon.png" width="96" align="right" alt="SCALE Console app icon">

# SCALE Console

Desktop application of the AAPM Working Group SCALE. It runs the SCALE tools as Docker containers on a site's own computer: the DICOM folder is only read, the tools have no network access, and the private workspace stays on that computer.

More: [medomics.ai · SCALE Console](https://www.medomics.ai/scale-console.html)

## Download (version 0.4.4)

| System | File | Size |
|---|---|---|
| Windows 10/11, x64 | [SCALE-Console-0.4.4-win-x64-setup.exe](https://github.com/oliviermorin0097/scale-console/releases/download/v0.4.4/SCALE-Console-0.4.4-win-x64-setup.exe) | 219 MB |
| macOS, Apple silicon | [SCALE-Console-0.4.4-mac-arm64.zip](https://github.com/oliviermorin0097/scale-console/releases/download/v0.4.4/SCALE-Console-0.4.4-mac-arm64.zip) | 229 MB |
| macOS, Intel | [SCALE-Console-0.4.4-mac-x64.zip](https://github.com/oliviermorin0097/scale-console/releases/download/v0.4.4/SCALE-Console-0.4.4-mac-x64.zip) | 235 MB |
| Linux, x86_64 | [SCALE-Console-0.4.4-linux-x86_64.AppImage](https://github.com/oliviermorin0097/scale-console/releases/download/v0.4.4/SCALE-Console-0.4.4-linux-x86_64.AppImage) | 224 MB |

SHA-256 checksums: [SHA256SUMS.txt](https://github.com/oliviermorin0097/scale-console/releases/download/v0.4.4/SHA256SUMS.txt). Setup steps: [GETTING_STARTED.md](https://github.com/oliviermorin0097/scale-console/releases/download/v0.4.4/GETTING_STARTED.md).

## What you need
- Docker Desktop 24 or newer (on Windows with WSL 2); no Docker account.
- 2 GB of memory for Docker, 1 CPU and 2 GB of free disk for the de-identification step.

## Notes
- Each download includes the SCALE De-identification tool 0.3.0, installed on first start without any internet download.
- This build starts as a test kit: site code TEST and synthetic test patients. Choose your own DICOM folder on the Home screen to process real data under your institution's approvals.
- The installers are not yet code-signed. Windows: **More info → Run anyway**. macOS: right-click the app → **Open**.
