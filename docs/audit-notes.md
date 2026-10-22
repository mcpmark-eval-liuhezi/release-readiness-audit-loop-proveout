# Audit Notes

## What the release-audit workflow is for

The [`release-audit`](.github/workflows/release-audit.yml) workflow runs on every push to this repository.

On each push, the single `audit` job:

1. Writes a one-line placeholder audit summary to `artifact/audit-summary.txt`.
2. Uploads that file as a workflow artifact named **audit-report**, which can be downloaded from the run's summary page.

This is a minimal prove-out of the "release readiness audit" loop: repository push, automated audit job, artifact capture, and downstream review activity, all checked end to end before the template is pitched to the team.
