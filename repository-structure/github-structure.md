# How to Structure GitHub for GitBook

To enable GitBook to read and parse your repository properly, you must follow a clean, specific file organization pattern. GitBook relies on standard Markdown files (`.md`) and a map file to generate the interface.

## Required Root Files
Every GitBook-compatible repository requires two primary files at the root level:
* **`README.md`**: Serves as the landing homepage of your documentation space.
* **`SUMMARY.md`**: Acts as the exact architecture map for your left-hand sidebar navigation.

## Directory Layout
It is highly recommended to group related files into subdirectories. For example, keeping architecture rules in a `repository-structure/` folder keeps your GitHub cleaner than throwing all files into the root directory.