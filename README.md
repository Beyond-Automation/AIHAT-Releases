# AIHAT — Infrastructure Health Audit Toolkit

[![Version](https://img.shields.io/badge/version-1.2.0-22b8f0)](https://github.com/Beyond-Automation/AIHAT-Releases/releases/tag/v1.2.0)
[![Platform](https://img.shields.io/badge/platform-Windows%2010%20%7C%2011-0078D4)](https://beyondautomation.io/aihat)
[![License](https://img.shields.io/badge/license-Freeware-27c96f)](LICENSE.md)
[![Publisher](https://img.shields.io/badge/verified%20publisher-Randall%20Lewis-27c96f)](SECURITY.md)

**Understand the machine. Identify risk. Know what to do next.**

AIHAT is a free, read-only Windows infrastructure health assessment tool from [Beyond Automation](https://beyondautomation.io). It evaluates essential operational and security signals and produces a professional local HTML report.

## Download AIHAT v1.2.0

**[Download the signed Windows installer](https://github.com/Beyond-Automation/AIHAT-Releases/releases/download/v1.2.0/AIHAT-v1.2.0-Setup.exe)**

Also download the [SHA-256 checksum](https://github.com/Beyond-Automation/AIHAT-Releases/releases/download/v1.2.0/AIHAT-v1.2.0-Setup.exe.sha256), or view the [complete v1.2.0 release](https://github.com/Beyond-Automation/AIHAT-Releases/releases/tag/v1.2.0).

Only download AIHAT from this repository or [beyondautomation.io/aihat](https://beyondautomation.io/aihat).

## What AIHAT assesses

- System and operating-system health
- Windows Update state
- Microsoft Defender, firewall, BitLocker, Secure Boot, TPM, and UAC
- Local administrator posture
- Network adapter, IP, gateway, DNS, connectivity, and latency

## Trust and privacy

- Digitally signed and timestamped
- Windows verified publisher: **Randall Lewis**
- No account required
- No telemetry
- No audit-result uploads
- Reports and logs remain on the assessed computer
- Read-only assessment; AIHAT does not remediate or change system configuration

AIHAT requires administrator elevation so it can read protected Windows security evidence. Review [SECURITY.md](SECURITY.md) and [PRIVACY.md](PRIVACY.md) for details.

## Install and use

1. Download the installer and checksum.
2. Verify that Windows displays **Verified publisher: Randall Lewis**.
3. Install AIHAT and approve the UAC prompt.
4. Select **Start Audit**.
5. Review the score and findings, then open the detailed report.

See the complete [Installation Guide](INSTALLATION.md) and [User Guide](USER-GUIDE.md).

## Verify the download

```powershell
$Expected = (Get-Content .\AIHAT-v1.2.0-Setup.exe.sha256).Split(' ')[0].Trim()
$Actual = (Get-FileHash .\AIHAT-v1.2.0-Setup.exe -Algorithm SHA256).Hash.ToLowerInvariant()

if ($Actual -ne $Expected) {
    throw 'AIHAT installer checksum validation failed.'
}

'AIHAT installer checksum verified.'
```

Published installer SHA-256:

```text
d6499b0d11984be5a13c641ae0a41ae52c8ab1986c50b11f02c6dfb7f13e37bc
```

## Documentation

- [Installation Guide](INSTALLATION.md)
- [User Guide](USER-GUIDE.md)
- [Privacy Notice](PRIVACY.md)
- [Security Policy](SECURITY.md)
- [Freeware License](LICENSE.md)
- [Support](SUPPORT.md)

## Important

AIHAT provides informational infrastructure-health findings. Results are not a compliance certification, security guarantee, warranty, or substitute for qualified professional judgment.

---

**Beyond Automation** · [Website](https://beyondautomation.io) · [LinkedIn](https://www.linkedin.com/company/beyond-automation-io)

Public proof. Private engineering core.
