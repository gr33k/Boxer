# Boxer 4.2.0 Beta 2 - thec0de continuation

This follow-up to [4.2.0 Beta 1](./RELEASE_NOTES_4.2.md) restores the original
sample demos, adds visible credits, and provides a working bug-report path.
The emulator engine and app identity are unchanged.

## Changes

- Restores the original Epic Pinball, Ultima Underworld, and X-COM demo
  gameboxes and the optional first-run sample-copy flow.
- Adds thec0de's two-glove app icon while retaining the original Boxer icon
  assets in the source tree.
- Help > About Boxer now credits original creator Alun Bestor, MaddTheSane's
  modern fork, thec0de.com continuation, and the DOSBox team. The old About
  text's fixed DOSBox 0.74 reference was removed.
- Report a Bug now opens [this fork's issue form](https://github.com/gr33k/Boxer/issues/new?template=bug_report.yml)
  instead of the legacy Boxer website. The form asks for reproducible steps,
  version, Mac details, and optionally a reviewed error report.
- Keyboard Preferences now names the correct macOS settings pane instead of
  displaying `(null)`. Its Accessibility button uses the modern System Settings
  destination on macOS 13+ while preserving the macOS 12 route.
- Existing local error reports may be found under
  `~/Library/Application Support/Boxer/Crash Dumps/`. Review and redact
  personal paths or information before sharing one publicly.

## Beta status

This remains a 4.2.0 prerelease, build 42002, not a stable 4.2.0 release.
The universal Intel/Apple Silicon build targets macOS 12 or newer. Local M1
testing on macOS 26.6.2 is not a claim of Intel, macOS 12-25, or M3 Pro
validation; those remain pending. The archive is ad-hoc signed, not Developer
ID signed or notarized, so macOS may require a one-time manual approval.
Please [report problems on GitHub](https://github.com/gr33k/Boxer/issues/new/choose).

Boxer was created by Alun Bestor and modernized by MaddTheSane. This
continuation is by thec0de.com; the DOSBox and DOSBox Staging teams built
the emulation engine. The program remains GPLv2; see [LICENSE](./LICENSE).
