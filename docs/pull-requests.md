# Pull Requests Documentation

## Overview

Pull requests (PRs) are a core collaboration feature in GitBase, allowing users to propose changes to a repository through a structured review process.

A pull request allows changes from one branch to be reviewed and discussed before being merged into another branch. Each pull request includes the proposed code changes, review comments, and approval status to help maintain code quality and collaboration.

## Creating a Pull Request

### From the Web Interface

1. Navigate to your repository's **Pull Requests** tab.
2. Select the source branch containing your changes.
3. Select the target branch where the changes should be merged (typically `main` or `master`).
4. Click **New Pull Request**.
5. Add a title, description, labels, and assignees.
6. Review the changes shown in the diff preview.
7. Click **Create Pull Request**.

After creating the pull request, assigned reviewers will be able to review the proposed changes and provide feedback.

## Reviewing a Pull Request

Reviewers can inspect the proposed changes and either approve the pull request or request additional changes.

A review can include:

- Reviewing the changed files and code differences
- Adding comments or discussion on specific changes
- Approving the pull request when changes are acceptable
- Requesting changes before the pull request can be merged

## Automatic Merge Detection

GitBase automatically checks whether a pull request can be merged into the target branch.

When a pull request is created or updated, GitBase analyses the changes and determines whether the pull request is ready to be merged.

The pull request can have one of the following merge states:

- **Ready to Merge** - GitBase has detected that the changes can be merged automatically. Users with the required permissions will see the **Merge** button.
- **Merge Conflicts** - The pull request contains changes that conflict with the target branch. The conflicts must be resolved before the pull request can be merged.
- **Branch Update Required** - The source branch is behind the target branch and must be updated before merging.

When conflicts or updates are required, resolve the issues in the source branch and push the changes back to GitBase. The pull request status will be automatically re-evaluated after new changes are received.

## Merging a Pull Request

Once a pull request has been reviewed and GitBase has confirmed it can be merged, users with the required permissions can merge the pull request.

Before merging, ensure that:

- All required reviews have been completed.
- GitBase shows the pull request as ready to merge.
- Any required testing or validation has been completed.

Click **Merge pull request** to integrate the changes into the target branch.

## Pull Request Status

Pull requests can have the following statuses:

- **Open** - The pull request is active and awaiting review or changes.
- **Approved** - Reviewers have accepted the proposed changes.
- **Changes Requested** - Reviewers have requested modifications before merging.
- **Merged** - The changes have been successfully integrated into the target branch.
- **Closed** - The pull request has been closed without merging.

## Permissions

Pull request actions depend on repository permissions:

- Users with repository write access can create pull requests.
- Users with review permissions can approve or request changes.
- Users with merge permissions can merge approved pull requests.