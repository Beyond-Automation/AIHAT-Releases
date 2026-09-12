# AIHAT Privacy Notice

Effective date: September 12, 2026

AIHAT v1.2.0 performs a local, read-only Windows infrastructure health assessment.

## Data processing

AIHAT reads system configuration and operational information required to evaluate system health, Windows Update, security, and networking. This can include:

- Computer and operating-system information
- Memory and disk information
- Windows Update state
- Microsoft Defender, firewall, BitLocker, Secure Boot, TPM, and UAC state
- Local administrator account names
- Network adapter, IP address, gateway, DNS, connectivity, and latency information

## Storage

Reports and logs are stored locally under:

`%LOCALAPPDATA%\Beyond Automation\AIHAT`

## No collection by Beyond Automation

AIHAT v1.2.0:

- Does not require an account
- Does not include telemetry
- Does not upload audit results
- Does not sell or share audit data
- Does not transmit reports or logs to Beyond Automation

The connectivity test makes an outbound request only to determine whether internet connectivity and DNS resolution work. Assessment evidence is not included in that request.

## User responsibility

Reports can contain sensitive infrastructure information. Users are responsible for protecting, sharing, retaining, and deleting reports according to their own security and privacy requirements.

## Contact

Privacy questions may be submitted through mailto:contact@beyondautomation.io.
