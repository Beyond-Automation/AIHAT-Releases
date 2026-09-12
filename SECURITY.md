# Security Policy

## Supported versions

| Version | Supported |
|---|---|
| 1.2.x | Yes |
| Earlier versions | No |

Only installers obtained from this official Beyond Automation release repository and identified by Windows as **Verified publisher: Randall Lewis** are supported.

## Reporting a vulnerability

Do not report security vulnerabilities through public GitHub issues.

Use GitHub private vulnerability reporting when available. If it is unavailable, use the security contact at https://beyondautomation.io/contact and clearly mark the message **AIHAT Security Report**.

Include:

- A clear description of the vulnerability
- The affected AIHAT version
- Steps to reproduce
- Potential impact
- Any suggested mitigation

Please allow reasonable time for investigation and remediation before public disclosure.

## Scope

Reports may include credential exposure, unsafe command execution, privilege-boundary problems, insecure file or registry handling, improper permissions, data leakage, signing failures, or vulnerable third-party dependencies.

## Product behavior

AIHAT requires administrator elevation to collect protected Windows security evidence. Version 1.2.0 performs read-only assessment and stores reports locally. It does not collect telemetry or upload audit data to Beyond Automation.
