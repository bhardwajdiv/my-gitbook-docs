# Advanced Syncing & Markdown

To maintain a healthy documentation platform, your team must adhere to strict maintenance workflows and clean formatting rules.

## Synchronization Pipeline Mechanics
The automatic webhook linkage ensures that your docs stay updated in real time. 

### Resolving Sync Interruptions
If your public GitBook URL does not update within a minute of a GitHub push, follow these troubleshooting checkpoints:
1. Validate that the modified filename matches the casing used in `SUMMARY.md` exactly.
2. Check your GitBook space integration logs for syntax formatting errors.
3. Confirm that you pushed your local commits to the correct tracking branch (`main`).

## Markdown Formatting Standards
* **Relative Path Mapping**: Always use relative file paths inside your repository (`./folder/file.md`) instead of absolute, hardcoded URLs.
* **Visual Scannability**: Use tables to break up dense numerical comparisons, and use code blocks to isolate shell inputs or config settings.