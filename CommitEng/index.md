---

# Commit Standards: Convention and Specification

## Overview

The **Conventional Commits** specification defines a clear convention for commit messages, providing a format that is readable by both humans and automated tools. It allows organizing the code history in a way that facilitates the automatic generation of changelogs, determines semantic versioning (SemVer) automatically, and efficiently communicates the nature of changes among team members and users.

### Commit Message Structure

The convention specifies that commit messages should be structured as follows:

```
<type>[optional scope]: <description>

[optional body]

[optional footer(s)]
```

## Commit Types

The specification defines the following commit types for commit messages:

- **`feat`**: A new feature or functionality added to the codebase. Corresponds to **MINOR** changes in semantic versioning.
  
- **`fix`**: A fix for an issue or bug in the codebase. Corresponds to **PATCH** changes in semantic versioning.
  
- **`docs`**: Changes related to project documentation.
  
- **`test`**: Modifications to tests, such as adding or updating them.
  
- **`build`**: Changes to dependencies, build configurations, or related tools.
  
- **`perf`**: Improvements to performance within the code.
  
- **`style`**: Changes that affect code formatting without changing functionality.
  
- **`refactor`**: Code changes that do not affect functionality but improve the structure.
  
- **`chore`**: Auxiliary tasks, such as modifying development tools or general configuration.
  
- **`ci`**: Changes to continuous integration configurations.
  
- **`raw`**: Changes related to file structures or data formats.
  
- **`cleanup`**: Removal of unused or obsolete code.
  
- **`remove`**: Removal of files or features.
  
- **`BREAKING CHANGE`**: Changes that break backward compatibility. Can be added as a footer or with the **`!`** symbol in the commit type.

## Example Commit Messages

- **Simple commit with type and description**  
  `feat: add support for additional languages`

- **Commit with type, scope, and BREAKING CHANGE**  
  `feat(api)!: introduce new user API structure`  
  `BREAKING CHANGE: the data structure has changed from JSON to XML.`

- **Commit with a detailed body**  
  `fix: fix discount calculation issue`  
  `The fix resolves an error that occurred when the discount was greater than the original price.`

- **Commit with footer, including ticket reference**  
  `fix: fix typo in the code`  
  `see the ticket for details on the typos fixed`  
  `Refs #123`

## Optional Footers

In addition to the description and body of the commit, you can include footers that provide additional context. Some examples include:

- **`BREAKING CHANGE`**: Used to indicate changes that break backward compatibility.  
- **`Closes`**: Used to close a ticket or issue, e.g., `Closes #123`.  
- **`Reviewed-by`**: Indicates who reviewed the commit, e.g., `Reviewed-by: John Doe`.

## Commit Message Rules and Specifications

The commit message **must** follow the defined structure, with a type followed by a clear description. The use of a scope is optional but recommended to provide more context. It is important to choose the commit type precisely to ensure that the version history is well-organized.

### Commit Requirements:

1. **Commit Type**: Must be a clear noun such as `feat`, `fix`, `docs`, etc.
2. **Scope (optional)**: Provides additional context about the part of the code affected, such as `feat(auth)` or `fix(parser)`.
3. **Description**: A brief, clear summary of the change.
4. **Body (optional)**: Detailed explanations or reasons for the change.
5. **Footer (optional)**: To provide additional information, such as ticket references or breaking changes.

## Why Use Conventional Commits?

- **Automation**: Enables the automated generation of CHANGELOGs.
- **Semantic Versioning**: Automatically determines the appropriate version increment (MAJOR, MINOR, PATCH).
- **Easy Collaboration**: Facilitates communication about changes within the project among team members and external contributors.
- **Automated Processes**: Can be integrated with CI/CD tools to trigger build, testing, and deployment processes.

## Frequently Asked Questions (FAQ)

1. **How should I handle commits during early development?**  
   Even during early development phases, it’s recommended to follow the convention, as it helps document progress and keeps the history organized.

2. **Should commit types be uppercase or lowercase?**  
   The choice between uppercase or lowercase is flexible, but consistency should be maintained throughout the project.

3. **What if a commit fits more than one type?**  
   Whenever possible, break the commits into more specific ones. Otherwise, use multiple types within a single commit and clearly document this in the body.

4. **Does this discourage fast development?**  
   The idea behind Conventional Commits is not to discourage fast development but to ensure that development is organized and well-documented, even during rapid iterations.

5. **How does Conventional Commits relate to SemVer?**  
   - `feat` → MINOR (new features)
   - `fix` → PATCH (bug fixes)
   - `BREAKING CHANGE` → MAJOR (incompatible changes)

## Final Considerations

Adopting the **Conventional Commits** specification is highly recommended for teams looking to maintain an organized code history, automate semantic versioning, and streamline changelog generation. Additionally, it helps communicate developer intentions more clearly, benefiting everyone involved in the software development lifecycle.

--- 
