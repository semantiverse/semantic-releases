# Semantic releases

Public binary releases and release notes for Semantic, a schema-driven semantic database.

[Download the latest release](https://github.com/semantiverse/semantic-releases/releases/latest)
or browse [all releases](https://github.com/semantiverse/semantic-releases/releases).
Each release lists its available platforms. The initial v0.0.1 release is Linux x86_64.

## Install and verify

Download the binary archive for your platform and `SHA256SUMS` from the same release.
On Linux, verify the downloaded archive before extracting it:

```sh
sha256sum --check --ignore-missing SHA256SUMS
tar -xzf semantic-v<VERSION>-<TARGET>.tar.gz
```

Put the extracted `semantic` executable on your PATH. The server embeds its web UI.
The Linux v0.0.1 binary requires glibc 2.39+ and standard C/compiler runtime libraries.
HEIC decoding uses pure Rust and needs no system codec packages.
Install FFmpeg (including ffprobe) for video processing and media probing.
See each release's notes and bundled third-party notices for further requirements.

## About this mirror

This repository contains release notes and built binaries. Release titles, notes,
prerelease status, and uploaded assets are copied from the primary release and
checked with SHA-256 before publication. The archive's `build-info.json` and
`semantic --version` identify the actual source commit used for the build.

Tags here refer to this repository's own history. GitHub's automatic **Source code**
archives contain this mirror's README, not application source or binaries.
Download the explicitly uploaded binary assets instead.
