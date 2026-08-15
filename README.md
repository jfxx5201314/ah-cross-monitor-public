# AH-Cross Monitor Mirror

Public, read-only, credential-safe mirror for the AH-Cross V0.4.0 production monitor.

- `monitor.json`: validation/automation/PML summary used for acceptance monitoring.
- `health.json`: compact status for quick checks.
- `.github/workflows/monitor-mirror.yml`: fetches production `/monitor.txt` every 15 minutes and updates the mirror only when content changes.

No API key, database URL, admin token, raw odds payload, or private credential is mirrored. The workflow uses an explicit allow-list of fields.
