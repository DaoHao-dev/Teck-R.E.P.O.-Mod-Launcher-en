# Contributing

## Bug reports

Open **Issues → New issue → Bug report** and include:

- Launcher version and R.E.P.O. version.
- Steps to reproduce, expected behavior, and actual behavior.
- Other installed mods, if any.
- Screenshots; for clipped text, include your resolution and UI scaling.

Remove unrelated personal information such as Steam IDs and private paths from screenshots or logs before posting publicly.

## Feature requests

Use the **Feature request** form to describe your use case and proposed change. For translation feedback, include the current label and your suggested wording.

## Source changes

Describe the change, its purpose, and the checks performed in your pull request. Read [SECURITY_NOTICE.md](SECURITY_NOTICE.md) before executing any build scripts. The current build script executes the compiled launcher for self-tests and preview generation; do not run it while the detection remains unresolved.

Editing the translation table alone does not update the embedded plugin. Translation changes require rebuilding the plugin and repackaging the affected mods; the launcher build embeds the packages already present.
