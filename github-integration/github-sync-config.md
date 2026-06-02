# Configuring GitHub Sync

Once linked, you must specify the precise directional mapping and file parsing boundaries for the automation engine.

## Alignment Parameters
You must declare target values for the three core sync configuration fields:

### 1. Default Working Branch
Explicitly lock the tracking branch targets to your primary production line. For modern repositories, this parameter should point directly to the `main` branch.

### 2. Root Asset Direction
Specify the path location within your project directory tree where GitBook should scan for files. Enter `./` to capture the absolute root folder level.