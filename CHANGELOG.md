# Changelog

## Distribution status — October 19, 2026

EXE distribution is paused following a Microsoft Defender detection. The cause is under investigation. See [SECURITY_NOTICE.md](SECURITY_NOTICE.md). The items below describe implemented features, not a verified safe binary release.

## v1.2.0 — October 19, 2026

### Interface

- PS1-inspired launcher with transparent desktop space around the console.
- Hinged lid animation and a spinning disc that can be paused.
- Custom application icon using the logo supplied by the project owner.
- Removed the session-information block and the Journal button from the console body.

### Language

- Added a VI / EN switch with a saved preference for GameTools and CosmeticsTools.
- Shortened the Vietnamese tabs to “Vật phẩm” and “Hiển thị.”
- Replaced untranslated Chinese language-switch labels and removed “Giao diện” from the button.

### Installation

- Embedded the prepared localized mod bundle in the launcher.
- Updated the installer to replace and verify managed plugin DLLs during updates.
- Prepared source files and a SHA256 file for the earlier build; a checksum identifies a file and does not establish its safety.

### Validation

Install/update/uninstall self-tests, translation tests, and language-button checks were performed. Full in-game behavior has not been verified, and the Defender detection remains unresolved.
