# Repositories Documentation

## Overview

GitBase provides a comprehensive repository management system, allowing you to host, organize, and collaborate on source code repositories.   
Each repository represents an independent Git project that can contain code, documentation, issues, pull requests, and other collaborative features.

## Repository Types

### 1. Private Repositories
Private repositories provide full access control over who can view and contribute to your project.
Ideal for sensitive source code that requires strict permissions.

**Access Control:**
- Owner has full administrative privileges
- Contributors, reviewers, and viewers can be assigned
- Repository visibility is hidden from public discovery

### 2. Public Repositories
Public repositories are visible to anyone who finds the repository. Suitable for:
- Open-source projects
- Documentation-heavy repositories
- Community-driven development
- Showcase portfolios

**Access Control:**
- Anyone can view, comment, and submit pull requests
- Forking is typically enabled by default
- Contribution workflow follows standard open-source practices

## Repository Operations

### Creating a New Repository
1. Tap the **+** button at the bottom of the screen
2. Select **New Repository**
3. Enter a descriptive repository name (alphanumeric characters, hyphens, underscores)
4. Enter the repository description (optional)
5. Select visibility: Private or Public
6. Choose initial files if desired (README.md, .gitignore)
7. Click **Create Repository**

### Cloning Repositories

GitBase repositories support standard Git protocols. Clone via:

```bash
# HTTP clone (recommended for most use cases)
git clone http://your-gitbase-git-server-address/repo-name.git
```

### Repository Structure

Each repository contains the following components:

- **Repositories**: The primary code storage and collaboration space
- **Issues**: Track bugs, feature requests, and tasks within a repository
- **Pull Requests**: Propose and review changes before merging into main branches
- **Releases**: Version control and distribution of code releases
- **Settings**: Configure repository-specific behaviors and permissions

## Repository Management Best Practices

1. **Naming Conventions**: Use clear, descriptive names following your organization's naming standards (e.g., lowercase-hyphenated-names)
2. **Branch Strategy**: Implement consistent branching strategies (GitFlow, Trunk-Based Development, GitHub Flow) as appropriate for your workflow
3. **Documentation**: Maintain README.md in every repository with setup instructions and usage examples
4. **Issue Management**: Keep issues updated with clear descriptions, reproduce steps, and priority labels
5. **Review Process**: Require code reviews for all pull requests to maintain quality standards

## Troubleshooting Common Issues

- **Repository not visible**: Check network connectivity and ensure the repository URL is correct
- **Pull requests failing**: Verify that contributors have write permissions on the target branch
- **Push rejections**: Ensure your local branch is up-to-date with the remote before pushing
- **Slow performance**: Check available storage space, consider using Git LFS for large files

## Team Management

### Adding Collaborators

You can add repository collaborators via the web ui:

1. Navigate to **The Repository** → **Settings tab** → **Collaborators tab**
2. Click **Add collaborator**
3. Enter the member's username or email address in the search
4. Click the add button to the right of their Usersname to assign them as a collaborator.

### Removing Team Members
1. Navigate to **The Repository** → **Settings tab** → **Collaborators tab**
2. Under **Assigned collaborators** find the user you wish to remove.
3. Click the remove button to the right of their Usersname to remove the user as a collaborator.

## Migration Guide

### From Other Git Hosting Services

Migration from GitHub, GitLab, or Bitbucket to GitBase follows these steps:

1. Clone the existing repository to your local machine
2. Configure GitBase as the remote URL: `git remote set-url origin https://your-gitbase-git-server-address/repo-name.git`
3. Push all history to GitBase: `git push origin --force-with-lease`
4. Re-create issues, pull requests, and release notes in GitBase

### From Local Development to GitBase

1. Initialize a new Git repository locally: `git init`
2. Configure GitRemote with your GitBase URL
3. Commit all existing changes and push them to GitBase
