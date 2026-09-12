# Installing AIHAT v1.2.0

## Download

Download both files from the [official AIHAT v1.2.0 release](https://github.com/Beyond-Automation/AIHAT-Releases/releases/tag/v1.2.0):

- `AIHAT-v1.2.0-Setup.exe`
- `AIHAT-v1.2.0-Setup.exe.sha256`

Do not download AIHAT from third-party mirrors.

## Verify the checksum

Open PowerShell in the download folder and run:

```powershell
$Expected = (Get-Content .\AIHAT-v1.2.0-Setup.exe.sha256).Split(' ')[0].Trim()
$Actual = (Get-FileHash .\AIHAT-v1.2.0-Setup.exe -Algorithm SHA256).Hash.ToLowerInvariant()

if ($Actual -ne $Expected) {
    throw 'AIHAT installer checksum validation failed.'
}

'AIHAT installer checksum verified.'
```

## Install

1. Double-click `AIHAT-v1.2.0-Setup.exe`.
2. Confirm that Windows identifies the verified publisher as **Randall Lewis**.
3. Select the installation location.
4. Optionally create a desktop shortcut.
5. Complete the wizard.
6. Leave **Launch AIHAT** selected or launch it later from the Start Menu.
7. Approve the Windows UAC prompt.

AIHAT installs under `C:\Program Files\Beyond Automation\AIHAT`. Administrative approval is required for installation and for each audit launch.

## Run an assessment

1. Select **Start Audit**.
2. Wait for all four collectors to finish.
3. Review the score and findings.
4. Select **Open Report** for detailed evidence.

Reports and logs are stored under:

`%LOCALAPPDATA%\Beyond Automation\AIHAT`

No audit information is transmitted to Beyond Automation.

## Uninstall

Open **Settings > Apps > Installed apps**, locate **AIHAT**, and select **Uninstall**.
