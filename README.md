# Pipeline downloads

This repository hosts public Pipeline downloads and download documentation.
Pipeline application source is maintained separately in a private repository.

## Download status

No production release is available yet. Publication and installed-app download
qualification are in progress. This repository's existence does not establish
macOS signing, notarization, installation or update acceptance.

When available, download the assets attached to a
[published release](https://github.com/Sprig-Aerospace/pipeline-releases/releases).
Public release listings and assets require no GitHub account, token, `gh`, or
developer tools. Files labeled **Source code** are archives of this download
documentation, not the Pipeline application.

## Release files

A complete production release will include the macOS application archive, DMG,
setup executable, signed `release.json` metadata, `release-checksums.txt`, and a
publication completion record. Only use a release after its applicable acceptance
is recorded. Preview releases are marked as prereleases; stable releases are not.

The installed updater checks signed metadata, artifact hashes, platform,
channel and release sequence. Downloading or preparing an update does not give
consent to activate it. Use the app's explicit **Update now** or
**Update on next launch** choice.

Anonymous downloads do not replace signature verification. A checksum list alone
is not the app's trust authority, and no download should require entering a
GitHub token.
