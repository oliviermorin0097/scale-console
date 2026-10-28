<img src="app-icon.png" width="96" align="right" alt="SCALE Console app icon">

# SCALE Console

Desktop application of the AAPM Working Group SCALE. It runs the SCALE tools as Docker containers on a site's own computer: the DICOM folder is only read, the tools have no network access, and the private workspace stays on that computer.

More: [medomics.ai · SCALE Console](https://www.medomics.ai/scale-console.html)

## Download (version 0.5.0)

| System | File | Size |
|---|---|---|
| Windows 10/11, x64 | [SCALE-Console-0.5.0-win-x64-setup.exe](https://github.com/oliviermorin0097/scale-console/releases/download/v0.5.0/SCALE-Console-0.5.0-win-x64-setup.exe) | 127 MB |
| Linux, x86_64 | [SCALE-Console-0.5.0-linux-x86_64.AppImage](https://github.com/oliviermorin0097/scale-console/releases/download/v0.5.0/SCALE-Console-0.5.0-linux-x86_64.AppImage) | 132 MB |

SHA-256 checksums: [SHA256SUMS.txt](https://github.com/oliviermorin0097/scale-console/releases/download/v0.5.0/SHA256SUMS.txt). Setup steps: [GETTING_STARTED.md](https://github.com/oliviermorin0097/scale-console/releases/download/v0.5.0/GETTING_STARTED.md). Test patients: [SCALE test data (2 fake patients)](https://github.com/oliviermorin0097/scale-console/releases/tag/testdata-v1).

## What you need
- Linux (Ubuntu 22.04 or newer): run `sudo apt install libfuse2` once before the first start of the AppImage.
- Windows 10/11 or Linux, with Docker Desktop or Docker Engine 24 or newer (on Windows with WSL 2); no Docker account.
- An NVIDIA GPU (8 GB or more) for step 4 Map to MNI. Without one, the other steps run and the de-identified release is sent to UCSF for step 4.
- Internet once: on first start the Console downloads its SCALE tools (about 5.5 GB with an NVIDIA GPU, about 0.5 GB without one).

## Notes
- The eight steps: Find cases · TG-263 names · De-identify · Map to MNI · Check quality · Add clinical data · Prepare submission · Build lesion maps. A person decides five times; everything else runs on its own.
- This build starts with the site code TEST. **Use the SCALE test data** on the Home screen to try it on fake patients; choose your own DICOM folder to process real data under your institution's approvals.
- Tested on Linux with NVIDIA GPUs. The Windows installer has not yet been run on a Windows computer: first Windows tests are in progress.
- The installers are not yet code-signed. Windows: **More info → Run anyway**.
