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

## Metadata trust bootstrap

The next access-qualification release introduces a replacement metadata signer.
Its public-key fingerprint is:

`76fe02c6af2fe2a905753a4b175332a10dd47e16d1409b510c419b11eec88dd3`

The prior public identity remains recorded for historical release verification:

`079eac60cd4d5c722432967bfd89faa31159c738bcd1cae93fe38af639ffa1af`

Existing installations do **not** trust a new-key-only update automatically.
They require an explicitly installed replacement app/installer obtained through
an independently trusted owner delivery/review step. The old updater cannot use
the new signature to authenticate its own trust replacement.

Quit the app and stop its owned service before replacement. Reuse the existing
managed installation layout and preserve profiles, settings, repositories and
workflow configuration. Existing enrolled release adapters need explicit
migration and a new review; old scheduled consent must not be replayed against
the changed helper/feed. Detailed migration acceptance is still in progress.

Public preview access-qualification assets are ad-hoc builds. They do not claim
Apple Developer ID signing or notarization, a clean-account installation result,
or second-machine/team readiness.
