# Boxer 4.2.0 Beta - thec0de continuation

This beta carries Boxer forward with the familiar app identity, the original
sample demos, a refreshed icon, and a build for current Macs. It builds on
Alun Bestor's original app and MaddTheSane's modern fork. The emulator engine
has not been rebased for this release.

## Changes

- Includes the original Epic Pinball, Ultima Underworld, and X-COM demo
  gameboxes and the optional first-run sample-copy flow.
- Adds thec0de's two-glove app icon while retaining the original Boxer icon
  assets in the source tree.
- Applies the saved-gamebox-path and shell-readiness fix from
  [upstream pull request #82](https://github.com/MaddTheSane/Boxer/pull/82).
- Help > About Boxer credits original creator Alun Bestor, MaddTheSane's
  modern fork, thec0de.com, and the DOSBox team.
- Report a Bug opens [this fork's issue form](https://github.com/gr33k/Boxer/issues/new?template=bug_report.yml).
  The form asks for reproducible steps, version, Mac details, and optionally
  a reviewed error report.
- Keyboard Preferences now names the correct macOS settings pane instead of
  displaying `(null)`. Its Accessibility button uses the modern System Settings
  destination on macOS 13+ while preserving the macOS 12 route.
- Modernizes the Xcode build workflow for the current toolchain.

## Beta status

This is a prerelease, build 42002, not a stable 4.2.0 release. The universal
Intel/Apple Silicon build targets macOS 12 or newer. The exact release ZIP
opened a DOS prompt and accepted keyboard input on an M1 Mac running macOS
26.6.2. The bundled Epic Pinball demo reached its menu, closed, and reopened
to the menu. Intel, macOS 12-25, and M3 Pro testing remain pending; the target
alone is not a compatibility guarantee.

The archive is ad-hoc signed, not Developer ID signed or notarized, so macOS
may require a one-time manual approval. Local error reports may be found under
`~/Library/Application Support/Boxer/Crash Dumps/`. Review and redact personal
paths or information before sharing one publicly. Please
[report problems on GitHub](https://github.com/gr33k/Boxer/issues/new/choose).

Boxer was created by Alun Bestor and modernized by MaddTheSane. This
continuation is by thec0de.com; the DOSBox and DOSBox Staging teams built
the emulation engine. The program remains GPLv2; see [LICENSE](./LICENSE).
