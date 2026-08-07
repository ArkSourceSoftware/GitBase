# Getting Started with GitBase

This guide will help you get started quickly and efficiently using GitBase.

## System Requirements

To run GitBase on your device, ensure the following requirements are met:

- **Android Version**: 8.0 (API level 26) or higher
- **Minimum Storage**: 500 MB free space
- **Network**: Wi-Fi or local network access is required when accessing repositories from other devices
- **RAM**: At least 1 GB available

## Installation

GitBase is available through the following channels:

### Google Play Store
1. Open the Google Play Store application on your Android device and search for "GitBase".   
   Alternatively, if you are viewing this page on your Android device, you can install it directly from the [Google Play Store](https://play.google.com/store/apps/details?id=com.arksource.gitbase).
2. Tap the GitBase app listing and select "Install"
3. Wait for the installation to complete. Installation time depends on your network speed and device.

## First-Time Setup

After installation, follow these steps to configure GitBase:

1. Open the GitBase application on your device.
2. Allow notifications when prompted.
3. Select **"New Setup"** and follow the on-screen instructions to create your administrator account and configure your GitBase server.
4. After setup is complete, GitBase will display the administrator sign-in screen along with the addresses for accessing the Git server and web interface.
5. Connect to GitBase using a web browser, Git CLI, an IDE, or a desktop Git client.

GitBase can operate entirely on your local network. No internet connection is required after installation.

## Creating Your First Repository

To create a new repository through the web interface:

1. Tap the **+** button at the bottom of the screen
2. Select **New Repository**
3. Enter a name for your repository
4. Choose whether to use Git (standard) or SVN (legacy support) as the version control system
5. Initialize the repository and create an initial commit with a message

## Using Git Commands

GitBase provides an integrated command-line interface for advanced Git operations:

- `git status`: Check the current state of your working directory
- `git log`: View commit history
- `git diff`: Compare changes between commits
- `git branch`: Manage branches
- `git merge`: Combine changes from different branches

## Backup and Restore

Protect your GitBase server by using the built-in Snapshot system.

Snapshots are complete backups of your GitBase server that can be used to restore a GitBase server or transfer it to a new device.

### Creating a Snapshot

1. In the GitBase application, navigate to **Administrator** → **Settings**.
2. Under **Database and Snapshots**, tap **Export GitBase Snapshot**.
3. Select a destination for the snapshot file.
4. The snapshot will be created. The time it takes will depend on your database size and device performance.

### Restoring a Snapshot

1. In the GitBase application, navigate to **Administrator** → **Settings**.
2. Under **Database and Snapshots**, tap **Restore GitBase Snapshot**.
3. Select an existing snapshot file.
4. The snapshot will be restored. The time it takes will depend on your database size and device performance.

> **Note:** Restoring a GitBase snapshot will overwrite all existing GitBase data.

### Migrating to a New Device

1. Create a snapshot on the existing device.
2. Transfer the snapshot file to the new device.
3. Install GitBase and restore the snapshot.
