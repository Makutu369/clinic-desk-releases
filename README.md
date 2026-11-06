# Clinic Desk releases

This repository hosts the desktop update artifacts for **Clinic Desk**
(Perfect Vision Eye Clinic). The source repository is private; only the built
binaries and their checksums are published here.

Releases are created by the `Release desktop app` workflow in the source
repository when a `v*` tag is pushed. Each release contains:

- `PerfectVisionEyeClinic-windows-amd64.exe` — portable Windows build used by
  the in-app updater.
- `PerfectVisionEyeClinic-windows-amd64-installer.exe` — Windows installer for
  first-time installs.
- `PerfectVisionEyeClinic-linux-amd64` — portable Linux build used by the
  in-app updater.
- `checksums.txt` — SHA-256 digests verified by the updater before an update is
  staged.

The app checks the latest release through the GitHub Releases API and prompts
inside its own update panel. Release notes are shown before downloading.
