<img src="app-icon.png" width="96" align="right" alt="SCALE Console app icon">

# SCALE Console

Desktop application of the AAPM Working Group SCALE. It runs the SCALE tools as Docker containers on a site's own computer: the DICOM folder is only read, the tools have no network access, and the private workspace stays on that computer.

More: [medomics.ai · SCALE Console](https://www.medomics.ai/scale-console.html)

## Download (version 0.5.2)

| System | File | Size |
|---|---|---|
| Windows 10/11, x64 | [SCALE-Console-0.5.2-win-x64-setup.exe](https://github.com/oliviermorin0097/scale-console/releases/download/v0.5.2/SCALE-Console-0.5.2-win-x64-setup.exe) | 128 MB |
| **Ubuntu / Debian** (recommended on Linux: double-click, Install) | [SCALE-Console-0.5.2-linux-amd64.deb](https://github.com/oliviermorin0097/scale-console/releases/download/v0.5.2/SCALE-Console-0.5.2-linux-amd64.deb) | 107 MB |
| Other Linux | [SCALE-Console-0.5.2-linux-x86_64.AppImage](https://github.com/oliviermorin0097/scale-console/releases/download/v0.5.2/SCALE-Console-0.5.2-linux-x86_64.AppImage) | 133 MB |

SHA-256 checksums: [SHA256SUMS.txt](https://github.com/oliviermorin0097/scale-console/releases/download/v0.5.2/SHA256SUMS.txt). Setup steps: [GETTING_STARTED.md](https://github.com/oliviermorin0097/scale-console/releases/download/v0.5.2/GETTING_STARTED.md). Test patients: [SCALE test data (2 fake patients)](https://github.com/oliviermorin0097/scale-console/releases/tag/testdata-v1).

## What you need
- Windows 10/11 or Linux, with Docker Desktop or Docker Engine 24 or newer (on Windows with WSL 2); no Docker account. If Docker is missing, the Console sets it up in one click (Windows: Docker Desktop and WSL 2, one approval and one restart).
- For step 4 Map to MNI: an NVIDIA GPU with about 32 GB of memory (a typical 512 × 512 × ~200 brain MRI needs about 28 GB). Without one, the other steps run and the de-identified release is sent to UCSF for step 4.
- Internet once: on first start the Console downloads its SCALE tools (about 5.5 GB with a suitable NVIDIA GPU, about 0.5 GB otherwise).

## Notes
- The eight steps: Find cases · TG-263 names · De-identify · Map to MNI · Check quality · Add clinical data · Prepare submission · Build lesion maps. A person decides five times; everything else runs on its own.
- This build starts with the site code TEST. **Use the SCALE test data** on the Home screen to try it on fake patients; choose your own DICOM folder to process real data under your institution's approvals.
- Tested on Linux with NVIDIA GPUs, on fresh Ubuntu 22.04 to 26.10, and in a Windows 11 virtual machine (setup, download, steps 1, 2, 3 and 6). First tests on physical Windows PCs are in progress.
- The Windows installer is not yet code-signed: **More info → Run anyway**.
