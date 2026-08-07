# Backup Management Guide

## Overview

GitBase includes a built-in Snapshot system that allows you to create complete backups of your GitBase server.

Snapshots can be used to:

- Protect your GitBase data from accidental loss
- Restore your server after reinstalling GitBase
- Transfer your GitBase server to a new device
- Maintain backup copies of your repositories and configuration

A GitBase snapshot contains all required data to restore your GitBase server to the state it was in when the snapshot was created.

## Creating a Snapshot

To create a backup of your GitBase server:

1. In the GitBase application, navigate to **Administrator** → **Settings**.
2. Under **Database and Snapshots**, tap **Export GitBase Snapshot**.
3. Select a destination for the snapshot file.
4. GitBase will create the snapshot.

The time required to create a snapshot depends on the size of your GitBase database and the performance of your device.

After completion, store the snapshot file in a safe location.

## Restoring a Snapshot

A snapshot can be restored to recover your GitBase server or migrate it to another device.

To restore a snapshot:

1. In the GitBase application, navigate to **Administrator** → **Settings**.
2. Under **Database and Snapshots**, tap **Restore GitBase Snapshot**.
3. Select an existing GitBase snapshot file.
4. Confirm the restore operation.

The restore process time depends on the size of the snapshot and the performance of your device.

> **Warning:** Restoring a GitBase snapshot will overwrite all existing GitBase data on the device.

## Migrating GitBase to a New Device

Snapshots make it possible to move your GitBase server between devices.

To migrate GitBase:

1. Create a snapshot on the existing device.
2. Transfer the snapshot file to the new device.
3. Install GitBase on the new device.
4. Restore the snapshot.
5. Verify that repositories, users, and settings have been transferred successfully.

## Backup Recommendations

To help protect your data:

- Create regular snapshots of your GitBase server.
- Store snapshots somewhere other than the device running GitBase.
- Keep multiple backup versions if your repositories are frequently changing.
- Test restoring a snapshot periodically to ensure backups are working correctly.

## Snapshot Storage

GitBase snapshots are stored as files that can be copied, moved, or archived like other files.

For long-term protection, consider storing snapshots in:

- Another device
- A computer
- External storage
- A secure cloud storage service

## Restoring After Data Loss

If your GitBase device is lost, damaged, or replaced:

1. Install GitBase on the replacement device.
2. Transfer your latest snapshot file to the device.
3. Restore the snapshot.
4. Confirm that your repositories and user accounts are available.