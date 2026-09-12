# AIHAT User Guide

## Start an audit

1. Open **AIHAT** from the Start Menu or desktop shortcut.
2. Approve the Windows UAC prompt.
3. Select **Start Audit**.
4. Wait for System Health, Windows Update, Security Health, and Networking Health to complete.
5. Review the score, module status, and findings.
6. Select **Open Report** to view the detailed HTML report.

## Status meanings

- **Healthy** — no warning or critical condition was detected.
- **Warning** — the assessment completed and identified something that should be reviewed.
- **Critical** — an important control or required capability failed.
- **Incomplete** — required evidence could not be collected; AIHAT intentionally withholds the score.

## Health score

A complete assessment starts at 100 and deducts points for warning or critical findings. The score is an operational summary, not a compliance certification, warranty, or substitute for professional judgment.

## Reports and privacy

Reports contain system and security configuration evidence and may include computer name, network addresses, local administrator names, and other environment details. Treat reports as sensitive operational information.

Reports and logs remain on the assessed computer under:

`%LOCALAPPDATA%\Beyond Automation\AIHAT`

AIHAT does not upload reports, collect telemetry, or require an account.

## Important limitations

AIHAT v1.2.0 is read-only. It reports conditions but does not enable BitLocker, install updates, change firewall settings, remove administrators, or perform remediation.
