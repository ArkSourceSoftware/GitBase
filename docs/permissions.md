# Permissions Documentation

## Overview

GitBase uses a permission system to control access to users, repositories, and administrative features.

Permissions determine what actions users can perform, such as creating repositories, managing users, pushing code, reviewing pull requests, and managing issues.

## User Roles

GitBase supports different user roles to control access across the server.

### Administrator

Administrators have full access to manage the GitBase server.

Administrators can:

- Create and manage users
- Manage repositories
- Configure GitBase settings
- Manage permissions
- Access all repository features

At least one administrator account must always exist.

### User

Regular users can interact with repositories based on the permissions granted to them.

Users can:

- Create and manage their own repositories (if enabled)
- Access repositories they have permission to view
- Create issues and pull requests
- Participate in repository discussions

## Repository Permissions

Repository permissions control what users can do within an individual repository.

Available permissions include:

### Read

Allows users to view repository contents.

Users with read access can:

- Browse repository files
- Clone repositories
- View issues and pull requests

### Write

Allows users to contribute changes to a repository.

Users with write access can:

- Push commits
- Create branches
- Create and manage issues
- Create pull requests

### Manage

Allows users to manage repository settings and contributors.

Users with manage access can:

- Change repository settings
- Manage repository permissions
- Manage branches and repository configuration

### Administrator

Provides full control over a repository.

Repository administrators can:

- Perform all repository actions
- Manage all users and permissions
- Delete the repository

## Pull Request Permissions

Pull request actions are controlled by repository permissions.

Users may be able to:

- Create pull requests
- Review pull requests
- Approve changes
- Merge pull requests

The ability to merge a pull request requires the appropriate repository permissions.

## Issue Permissions

Issue access follows repository permissions.

Users with access to a repository may be able to:

- Create issues
- Comment on issues
- Assign users
- Edit or close issues

## Managing Repository Access

Repository administrators can grant or remove user access from the repository settings.

When granting access, select the appropriate permission level based on the actions the user needs to perform.

## Best Practices

For secure repository management:

- Grant users the minimum permissions required for their role.
- Use separate administrator accounts instead of sharing credentials.
- Review repository access permissions regularly.
- Avoid granting administrative access unless required.