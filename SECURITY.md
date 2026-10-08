# Security Policy for agent-audit-action

## Supported Versions

| Version | Supported          |
| ------- | ------------------ |
| v1.x    | :white_check_mark: |

## Security & Verification Standards

`agent-audit-action` runs `agent-audit` inside your GitHub Actions CI pipeline as a deterministic security gate.

1. **Pinned Actions & Least Privilege:**
   - The action recommends pinning to immutable commit SHAs in production workflows.
   - Requires only `contents: read` permissions.

2. **Zero Exfiltration:**
   - The action does not transmit code, git diffs, dependency names, or scan findings to any external third-party server.
   - All SARIF reports and exit codes are generated locally inside the runner.

## Reporting a Vulnerability

Please report security issues privately via GitHub Security Advisories or contact `mo9652962-ai@users.noreply.github.com`.
