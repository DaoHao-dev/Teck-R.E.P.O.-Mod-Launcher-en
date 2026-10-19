<div align="center">
  <img src="assets/teck-logo.png" width="112" alt="Teck logo">
  <h1>TECK</h1>
  <p><strong>R.E.P.O. Mod Launcher</strong></p>
  <p>A classic console design. One place to manage your mods.</p>
  <img src="docs/images/project-status.svg" width="460" alt="Windows · VI / EN · v1.2.0">
  <p>
    <a href="#preview">Preview</a> ·
    <a href="#features">Features</a> ·
    <a href="docs/USER_GUIDE.md">User guide</a> ·
    <a href="CHANGELOG.md">Changelog</a>
  </p>
</div>

---
## 📥 Download

## 📥 Download

You can download the latest version of the launcher here:

* **[Download Teck-PS1-VI-EN.exe](https://github.com/DaoHao-dev/Teck-R.E.P.O.-Mod-Launcher-en/raw/main/release-files/Teck-PS1-VI-EN.exe)**
* [Download SHA256 Checksum File](https://github.com/DaoHao-dev/Teck-R.E.P.O.-Mod-Launcher-en/raw/main/release-files/Teck-PS1-VI-EN-SHA256.txt)

> ⚠️ **Note regarding Windows Defender:** 
> Direct distribution of the `.exe` file is currently flagged by Microsoft Defender as a false positive (common for PyInstaller-packed or unsigned executables). If your antivirus blocks it, you can safely allow it to run or inspect the source code to build it yourself.

**Teck** is a Windows mod launcher for R.E.P.O., with an interface inspired by the original PlayStation. Open the lid to reveal a spinning disc, and use the console's buttons to install mods, adjust settings, and launch the game.

## Preview

![Teck launcher with the lid open and disc visible](docs/images/launcher-open.png)

<details>
<summary><strong>View the closed-lid design</strong></summary>

![Teck launcher with the lid closed](docs/images/launcher-closed.png)

</details>

*Images are exported from the launcher. The area outside the console is transparent on the desktop.*

## Features

| Feature | Details |
| --- | --- |
| **Classic console interface** | PS1-inspired shell, animated lid, spinning disc, pixel typography, and custom Teck icon. |
| **Mod management** | Install, update, or uninstall the bundled mod files managed by the launcher. |
| **Group settings** | Configure 2–20 players through MorePlayers and adjust shared-upgrade settings. |
| **In-game tools** | Open GameTools with F4 and CosmeticsTools with F5. |
| **Vietnamese / English** | Use VI / EN in the two mod menus to switch languages and save your preference. |

Actual player limits and mod behavior depend on the game version and the mods used by the lobby.

## Availability

This repository currently provides source files and documentation for review. **The flagged EXE is not included in this upload package.** No verified replacement binary is available from this package.

The [user guide](docs/USER_GUIDE.md) documents the intended controls and installation process. It is not a recommendation to run the flagged build.

## Bundled components

| Component | Version | Purpose |
| --- | --- | --- |
| BepInExPack | 5.4.2305 | Plugin loading |
| MorePlayers | 1.1.0 | Configurable player limit |
| SharedUpgradesPlus | 1.6.1 | Shared upgrades |
| MenuLib | 2.5.2 | Menu library |
| REPOConfig | 1.2.6 | Mod configuration |
| GameTools | 1.0.9 | In-game tools |
| CosmeticsTools | 1.0.1 | Cosmetics and cosmetic tokens |
| Teck Vietnamese | DLL 1.2.0 | Translation and VI / EN switching |

See [third-party acknowledgments](THIRD_PARTY.md) for authors, sources, and font information. The project owner supplied the Teck logo.

## Requirements and validation

Designed for Windows with **.NET Framework 4.x**, a Steam installation of R.E.P.O., and a game version compatible with the bundled mods.

Validation has covered install/update/uninstall behavior in a test directory, translation tests, language-button dispatch, and width measurements for the shortened labels. Full in-game behavior and layout have not been independently verified. Functional tests do not establish malware safety; see the security notice for the limits of the checks performed.

## Source layout

| Path | Contents |
| --- | --- |
| `src/TeckPS1Launcher.cs` | Combined launcher source |
| `src/localization/` | Translation table and localization support source |
| `assets/` | Console artwork, app icon, and font |
| `localized-packages/` | Previously prepared mod packages embedded by the build script |
| `build.ps1` | Launcher compilation, self-tests, and preview generation |

**Build caution:** `build.ps1` executes the resulting EXE for self-tests and preview generation. Do not run it while the detection remains unresolved. Rebuilding does not establish that the application is safe. Source and scripts can be reviewed without executing them.

The build script embeds existing localized packages; it does not recompile the translation plugin when its source or translation table changes.

## Feedback

Use **Issues** to report a bug or suggest an improvement. See [contribution guidelines](CONTRIBUTING.md) for the details to include.

---

<div align="center">
  <strong>TECK · A little nostalgia before every session.</strong>
  <p>A community project. Not affiliated with Sony, PlayStation, or the developers of R.E.P.O.</p>
</div>
