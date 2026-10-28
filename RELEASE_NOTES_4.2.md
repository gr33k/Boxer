# Boxer 4.2.0 - thec0de continuation

Boxer 4.2.0 continues MaddTheSane's fork of Alun Bestor's Boxer, with the
existing DOSBox Staging 0.78.1-era engine. This is a focused maintenance
release, not the proposed DOSBox Staging 0.83 migration or a Boxer 5.0 rewrite.

## Changes since the upstream source snapshot

- Restore the public Boxer's `net.washboardabs.boxer` app identity and related
  helper identities, so the fork does not adopt a contributor's test identity.
- Adopt the saved-gamebox-path and shell-readiness correction from upstream
  pull request [#82](https://github.com/MaddTheSane/Boxer/pull/82). The basic
  close/reopen path was tested; every historical saved-path variant was not.
- Set version 4.2.0 (build 42001) and build a universal Intel/Apple Silicon app
  with a macOS 12.0 deployment target.
- Disable the inherited automatic update check against the upstream development
  feed. The app's Releases menu opens thec0de Boxer website instead.
- Modernize the CI build configuration for current Xcode without changing the
  original fork's default branch.

## Distribution and compatibility

This build is ad-hoc signed, not Developer ID signed or notarized. macOS
Gatekeeper rejects it on first assessment, so a user may need to approve it
manually in macOS. Do not treat a successful `codesign --verify` as a
Gatekeeper pass. It has been tested on an M1 Mac running macOS 26.6.2; Intel,
macOS 12-25, and the owner's M3 Pro on macOS 26.7.1 remain untested. A release
build targets macOS 12+, but that target alone does not prove runtime support
on every older macOS version.

The original 4.1 Beta and older generation downloads remain separate.

## Source and credits

This project is GPLv2. The matching public release tag and source archive
contain the application source, build configuration, and pinned dependency
submodules. Preserve the included license notices and users' rights to modify
and redistribute the program. Boxer was created by Alun Bestor; MaddTheSane
maintained the modern fork; DOSBox and DOSBox Staging contributors built the
emulation engine. This 4.2 continuation is by thec0de.com.
