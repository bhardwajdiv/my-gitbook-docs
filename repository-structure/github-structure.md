# GitHub File Organization

To enable the GitBook parsing engine to read, interpret, and visually render your repository correctly, you must adhere to a strict file organization hierarchy. GitBook treats your repository as a systematic directory tree.

## Required Root-Level Core Files
Your repository must contain two essential configuration files located strictly at the absolute root directory path (`./`):

### 1. The Homepage (`README.md`)
The root `README.md` file serves as the absolute entry point and landing page of your published documentation space. If this file is missing or misplaced inside a sub-folder, the GitBook builder will fail to compile the home view and throw a deployment error.

### 2. The Architecture Map (`SUMMARY.md`)
The `SUMMARY.md` file functions as the blueprint file for your site navigation. Without this file, GitBook cannot determine your site tree, causing it to display a completely flat or unindexed list of loose files.

## Designing a Scalable Folder Structure
Throwing all `.md` files into the root directory creates a messy repository that is hard to maintain. Instead, isolate related content domains into functional, lower-case subdirectories.

### Recommended Production Blueprint:
* `repository-structure/`: Houses all structural tracking rules.
* `navigation/`: Dedicated to indexing, mapping, and user-experience guidelines.
* `best-practices/`: Stores syntax styling, table schemas, and deployment assets.