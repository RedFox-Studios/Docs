# Employee Guidelines for Tagging and Releases

## Introduction

Welcome to the **RedFox Studios** employee guidelines for repository management! If you work at RedFox Studios and have a repository within our organization, please follow the instructions below regarding tags and releases.

## Tagging and Releases

To maintain clarity and organization across our projects, we ask all employees to adhere to the following conventions when creating tags and releases:

### Tags
- **Format**: Tags should be formatted as follows: `v1.0`
  - Example: `v1.0`, `v1.1`, `v2.0`, etc.
  
### Releases
- **Format**: Releases should be formatted as follows: `Version 1.0`
  - Example: `Version 1.0`, `Version 1.1`, `Version 2.0`, etc.

## Purpose

By implementing this tagging and release strategy, we aim to achieve the following:
- **Better Overview**: Having a consistent tagging and release format helps in tracking progress and changes across our projects.
- **Order and Clarity**: Clear versioning allows team members to quickly identify the current state of a project and facilitates smoother collaboration.

## Best Practices for Tagging and Releases
- **Semantic Versioning**: 
  - Follow semantic versioning principles:
    - **MAJOR** version for incompatible changes,
    - **MINOR** version for backward-compatible functionality,
    - **PATCH** version for backward-compatible bug fixes.

- **Release Notes**:
  - Include brief release notes summarizing changes, new features, and bug fixes when creating a release.

- **Keep It Up to Date**:
  - Always update the version number before pushing changes to production.

## Examples
- **Creating Tags**:
  - Use the following command in Git:
    ```bash
    git tag v1.0
    git push origin v1.0
    ```

- **Creating Releases**:
  - Specify the tag and provide a description when creating a release in GitHub.

## Communicating Changes
- **Team Notifications**:
  - Notify your team when a new tag or release is created via your team's communication channel.

- **Documentation Updates**:
  - Ensure relevant documentation is updated for significant changes in releases.

## Conclusion

Thank you for your cooperation in following these guidelines. Your efforts help us maintain a well-organized and efficient development environment at RedFox Studios!

If you have any questions or need assistance with tagging or releases, please reach out to your team lead or the organization admins.
