# Teck user guide

> EXE distribution is paused while a Defender detection is investigated. These instructions document intended behavior; they are not a recommendation to run the flagged build. Read the [security notice](../SECURITY_NOTICE.md).

## Intended installation workflow

1. Close R.E.P.O. and open Teck.
2. Select **1 / THIẾT LẬP** (Settings).
3. Choose the game directory containing `REPO.exe` and `REPO_Data`.
4. Configure the player limit from 2–20 and the shared-upgrade options, including the 0–100% sharing chance.
5. Select **RESET / CÀI MOD** (Install mods) and wait for completion.
6. Select **POWER / MỞ GAME** (Launch game) to open R.E.P.O. through Steam.

The launcher controls retain their current labels. English names in this guide explain those labels; translating this documentation does not change the application itself.

## Console controls

| Control | Function |
| --- | --- |
| POWER | Launch R.E.P.O. through Steam |
| RESET | Install or update the mod bundle |
| OPEN | Open or close the lid |
| Disc, with lid open | Pause or resume rotation |
| Port 1 | Game selection, player settings, shared upgrades, and uninstall |
| Port 2 | Help |
| F4 / MOD, F5 / XU | Show instructions for the corresponding in-game menus |
| − / × | Minimize / close the launcher |

Drag an empty area of the console body to move the window.

## In-game menus and language

- **F4:** GameTools.
- **F5:** CosmeticsTools, including cosmetics and cosmetic tokens.
- **VI / EN:** Switch Vietnamese/English in these two mod menus and save the preference.

Press the function keys inside the game to open the menus. The F4/F5 controls on the launcher show help. If another mod uses the same key, check its key bindings.

## Updates and uninstalling

Intended update workflow: close the game, open the new launcher build, select RESET / CÀI MOD, then restart the game after installation completes. This workflow should only be used after a verified release becomes available.

To uninstall the managed bundle, close the game and use the uninstall control in Settings. The installer tracks its own files and restores backed-up files where available.

## Troubleshooting

| Symptom | Check |
| --- | --- |
| Game directory is rejected | Select the directory directly containing REPO.exe and REPO_Data. |
| Old translation remains after an update | The game must be fully closed before the updated DLLs are installed. |
| F4/F5 does not open a menu | Check installation status and conflicting key bindings. |
| Menu text is clipped | Include a screenshot, resolution, and UI scaling in your issue. |
| Defender reports a threat | Follow the security notice; do not bypass the detection. |

See [contribution guidelines](../CONTRIBUTING.md) for bug reports.
