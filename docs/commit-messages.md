# Commit Message Guidelines

## Introduction

Consistent and descriptive commit messages are essential for maintaining a clean and organized version history. This guide will provide you with guidelines for writing meaningful commit messages that follow the Conventional Commits specification.

## Commit Message Format

Each commit message should follow the format:

```xml
<type>(<scope>): <description>
<BLANK LINE>
[optional body]
<BLANK LINE>
[optional footer(s)]
```

The commit message contains the following structural elements to communicate intent to consumers of your library:

- **Type**: The type indicates the purpose of the commit and helps categorize the changes. Here are some commonly used types:

  - **feat**: Introduces a new feature to the codebase.
  - **fix**: Fixes a bug in the codebase.
  - **chore**: Performs maintenance tasks or other changes not related to code.
  - **docs**: Updates documentation.
  - **style**: Makes code style changes, such as formatting or indentation.
  - **refactor**: Applies code changes that do not affect behavior or functionality.
  - **perf**: Implements performance improvements.
  - **test**: Adds or modifies tests.
  - **ci**: Makes changes to the continuous integration configuration.

- **Scope** (optional): The scope provides additional contextual information about the commit. It represents the module, component, or section of the codebase related to the changes. For example, you can have a scope like "(parser)" or "(validation)".

- **Description**: The description is a concise summary of the changes introduced by the commit. It should be clear, meaningful, and written in the imperative mood. For example, "Add ability to parse arrays" or "Fix email validation regex".

- **Body** (optional): The body provides more detailed information about the changes made in the commit. It can include the motivation behind the changes, additional context, and any relevant details. The body should start one blank line after the description and can consist of multiple paragraphs. You can use the body to explain the reasoning behind a specific implementation choice, provide examples, or describe any notable considerations.

- **Footer** (optional): The footer is used to reference issues or provide other related information. It can include breaking changes, references to GitHub issues, or any other relevant information. For example, you can include a footer like "BREAKING CHANGE: The `sendEmail` function signature has changed" to indicate a breaking change.

## Examples

Here are some examples of well-formed commit messages:

```
feat(parser): Add ability to parse arrays
```

```
fix(validation): Fix email validation regex
```

```
docs(readme): Update installation instructions
```

```
chore(dependencies): Update package dependencies
```

```
test(api): Add unit tests for the API module
```

```
refactor: Simplify the configuration code
```

For commits that introduce breaking changes, you can use the following format:

```
feat!: Send an email to the customer when a product is shipped

BREAKING CHANGE: The `sendEmail` function signature has changed.
```

```
fix(validation)!: Update validation logic for email input

BREAKING CHANGE: The validateEmail function has been removed. Please use the new validateInput function with the email validation type instead.
```

## Conclusion

By following these commit message guidelines based on the Conventional Commits specification, you can ensure that your version history remains organized and easy to understand. Consistent commit messages improve collaboration and help in maintaining a clean and transparent development process. If you have any questions or need assistance, feel free to reach out to the team.

Happy committing!
