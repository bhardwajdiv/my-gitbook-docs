# Troubleshooting GitHub Sync

If a code change pushed to your cloud engine fails to update the live presentation layer, perform these troubleshooting verification steps.

## Common Pipeline Failure Modes

### 1. Casing Mismatches
The parsing compiler is strictly case-sensitive. If a folder path is declared as `Getting-Started/` in your local directory but written as `getting-started/` inside your navigation config, the webhook will crash.

### 2. Target Branch Out-of-Sync
Verify that your local system git commits are being pushed directly upstream to the precise branch monitored by the webhook configuration (`main`).