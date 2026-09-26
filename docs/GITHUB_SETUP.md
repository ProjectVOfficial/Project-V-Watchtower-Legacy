# Publishing Project V // Watchtower on GitHub

## Repository structure

This repository is the public Project V // Watchtower documentation and release hub.

The normal Git history contains documentation, attribution, issue templates, screenshots, and licensing information. Compiled Windows binaries belong in GitHub Releases rather than ordinary Git history.

## Official repository

`https://github.com/ProjectVOfficial/Project-V-Watchtower`

## Binary release assets

A Windows release may include:

- NSIS installer
- MSI installer
- standalone / portable executable
- checksum manifest
- release notes

The release page can visually emphasize the Windows executables.

## AGPL corresponding source requirement

Watchtower is a substantially modified downstream AGPL-covered work.

If Project V distributes object-code binaries, the corresponding source for the exact released build must also be made available in a compliant way.

For GitHub download releases, the simplest release practice is:

1. upload the Windows binaries;
2. upload the exact corresponding-source archive for the same build;
3. include the AGPL license and required upstream notices in that source archive;
4. link [UPSTREAM_AND_LICENSE.md](../UPSTREAM_AND_LICENSE.md) from the release description.

The source archive does not need to be the main or first download button, but it must remain available as required by the license.

## Release review

Before publishing a release:

- confirm the release version and tag;
- confirm installer filenames and architecture;
- confirm the binaries were tested;
- confirm checksums;
- inspect the corresponding-source archive;
- confirm no API keys, private databases, credentials, updater keys, or certificate private keys are present;
- confirm `LICENSE`, `NOTICE.md`, and upstream attribution are included;
- disclose unsigned status when applicable;
- confirm the release description does not imply World Monitor endorsement.

## GitHub-generated source archives

GitHub automatically generates `Source code (zip)` and `Source code (tar.gz)` links for a tag.

Those automatic archives only count as application corresponding source if the actual application source needed to build that release is present in this repository at that tag.

Because the current public repository is documentation-focused, do not rely on the automatic tag archives as the Watchtower application source unless the repository layout changes.

## Local repository remote

After the repository transfer to ProjectVOfficial, local Watchtower clones should use:

```powershell
git remote set-url origin https://github.com/ProjectVOfficial/Project-V-Watchtower.git
git remote -v
```
