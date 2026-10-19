# Windows Defender detection notice

**Status: under investigation. EXE distribution is paused.**

## What was reported?

On October 19, 2026, Microsoft Defender flagged `Teck-PS1-VI-EN.exe` as **Trojan:Win32/Bearfoos.A!ml**, with **Severe** severity. The detection was reported after the EXE was created. The Protection history screenshot showed **Restored**, which means the file was returned from quarantine; this does not indicate that it was verified as safe.

## Why did Defender flag it?

The specific cause has not been established. There is no Microsoft analysis result confirming either malware or a false positive.

The launcher bundles a mod loader, third-party mod DLLs, and a translation plugin. Installation writes these components into the selected game directory. This describes the application's behavior; **it does not prove that these behaviors caused the detection**. Being unsigned or being a modding tool is also insufficient to conclude that the alert is a false positive.

## Checks performed and their limits

- A Microsoft Defender scan of the existing mod-package directory reported “found no threats.” This result applies only to that scan and does not establish the safety of the complete EXE.
- The separate EXE scan did not complete and returned `0x80508023`. This is not a clean scan result.
- Build, translation, and install/update/uninstall tests check functionality, not malware safety. Some previous builds were executed for testing.
- There is no Microsoft verdict, and a complete security analysis of all third-party components has not been completed.

## Current handling

- Distribution of the flagged EXE is paused. This upload package contains source files and documentation for review, without the flagged EXE.
- Users are not asked to disable Defender, add exclusions, or restore the flagged file.
- If you have the EXE, stop running it and use Windows Security to quarantine or handle the detection. If you ran it, perform a full scan; Microsoft Defender Offline is an additional scanning option.
- A sample can be submitted to Microsoft for analysis. No submission case number or analysis result is available to report at this time.

Rebuilding, renaming the file, or not seeing the alert on another computer does not establish safety. Distribution status will only be updated when additional verification evidence is available; there is no confirmed date for resuming EXE releases.

## References

- [Microsoft's Bearfoos.A!ml entry](https://www.microsoft.com/en-us/wdsi/threats/malware-encyclopedia-description?name=Trojan%3AWin32%2FBearfoos.A%21ml)
- [Understanding Protection history](https://support.microsoft.com/en-us/windows/security/windows-security/protection-history-in-the-windows-security-app)
- [Submit a sample to Microsoft](https://www.microsoft.com/en-us/wdsi/filesubmission)
- [Microsoft Defender Offline](https://learn.microsoft.com/en-us/defender-endpoint/microsoft-defender-offline)
