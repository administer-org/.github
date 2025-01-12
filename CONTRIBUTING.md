# Contributing to Administer

Welcome to the Administer Contribution Guide! We are happy to have your interest in our project. This document oulines the guidelines for contributing to our projects, ensuring an enjoyable experience for everyone and ensure our maintainers are able to quickly and efficiently address your issues and merge requests.

---

## Table of Contents

- [Contributing to Administer](#contributing-to-administer)
  - [Table of Contents](#table-of-contents)
  - [Code of Conduct](#code-of-conduct)
  - [How to Contribute](#how-to-contribute)
    - [Reporting Issues](#reporting-issues)
    - [Suggesting Features](#suggesting-features)
    - [Contributing Code](#contributing-code)
    - [Improving Documentation](#improving-documentation)
    - [Adding/Improving Localizations](#addingimproving-localizations)
  - [Development Guidelines](#development-guidelines)
    - [Coding Standards](#coding-standards)
    - [Commit Messages](#commit-messages)
  - [Community Support](#community-support)
  - [License](#license)

---

## Code of Conduct

We are committed to providing a welcoming and inclusive environment. By participating, you agree to abide by our [Code of Conduct](./CODE_OF_CONDUCT.md). Please read it before contributing.

---

## How to Contribute

### Reporting Issues

If you encounter bugs, glitches or other issues please:
1. Check the [issue tracker](https://github.com/administer-org/issues) to see if it's already reported.
2. Open a new issue, providing:
    - A clear, descriptive title.
    - Steps to reproduce the issue.
    - Expected vs. actual behavior.
    - Relevant logs, screenshots, or code snippets of applicable.

If you believe it is a bug with Roblox rather than Administer please report it to them, we cannot do anything about it.

### Suggesting Features

Have an idea for the Administer ecosystem? Share it with us by:
1. Searching the [issue tracker](https://github.com/administer-org/issues) first to see if it has already been suggested.
2. Opening a feature request issue, describing:
    - The problem your feature solves.
    - Your proposed solution.
    - Any alternative approaches considered.

Alternatively, you can open [a ticket in our Discord server.](https://administer.notpyx.me/to/discord)

### Contributing Code

1. **Fork the Repository**: Click the "Fork" button at the top of the repository page.
2. **Clone Your Fork**:
   ```bash
    git clone https://github.com/your-username/repository-name.git
    cd repository-name
   ```
3. **Create a Branch**: Use a descriptive name (for example,`fix-typo-in-readme` or `create-notification-card`)
    ```bash
    git checkout -b branch-name
    ```
4. **Make Changes**: Make sure to follow our [development guidelines](#development-guidelines).
5. **Push Your Changes:**
    ```bash
    git push origin branch-name
    ```
6. **Submit a Pull Request**: Open a PR on the original repository, linking it to the issue it addresses (if applicable).

### Improving Documentation

You can help by correcting typos, improving clarity or adding examples. The process for contributing documentation is the same as contributing code.

### Adding/Improving Localizations

We welcome changes or additions to translations or other localization. We do not have a system such as weblate but you are welcome to add or modify changes to the translation folder. Please do not contribue if you do not natively understand the target language, do not use automated translators (Google Translate, Apple Translate app, Yandex, ...) to push translations.

---

## Development Guidelines

### Coding Standards

- Follow the style of existing code in the project.
- Write clear, maintainable, and self-descriptive code. Use comments if necessary.
- Use the standard variable naming convention for languages (PascalCase in Lua, camelCase in Java/TypeScript, snake_case in Python)
  
### Commit Messages

- Use clear, concise messages.
- Structure:
  ```
  <type>(<optional scope>): <description>
  
  [Optional body]

  [Optional footer]
  ```

- Commit Types:
  - `feat` Adds or removes a feature
  - `fix` Fixes one or more bugs/issues
  - `refacor` Rewrite or restructure a piece of code without changing behavior
  - `perf` A variant of `refactor` that improves performance
  - `docs` Changes documentation
  - `improvement` Improves an existing feature with better UX or alike
  - `style` Improving the code style (white-space, formatting, etc)

- Scopes:
  - Optional, used to provide more context
  - Tailored to each repo
  - Don't use issue identifiers as scopes

- Breaking Changes Indicator
  - Indicate breaking changes with a `[!!]` before the `:` in the subject line.
  - Example: `feat(button) [!!]: remove events`

- Description
  - Mandatory part of the format
  - Use imperative, present tense "change" not "changed" or "changes"
  - Don't capitalize the first letter
  - No period (`.`) at the end

- Body
  - Optional, used to describe motivation
  - Use imperative, present tense "change" not "changed" or "changes"
  - This is where issue identifiers and their relations are put

- Footer
  - Optional, include any information about breaking changes
  - Optionally reference an issue with its identifier (ex. `Fixes #2`)
  - Breaking changes should start with `BREAKING CHANGE:` followed by a space, the rest of the commit message is then used for breaking changes

Examples:
- ```
  feat: add new button properties
  ```

- ```
  feat(api): add new endpoint for monitoring statistics
  ```

- ```
  feat [!!]: remove button events

  addresses #33

  BREAKING CHANGE: buttons no longer fire callbacks.
  ```

- ```
  fix(button): fix wrong anchor point
  ```

- ```
  refactor(prompt): change how buttons are parented
  ```

### Pull Requests

- Reference relevant issues in your PR description (as described above).
- Ensure your branch is up-to-date with the `main` branch:
  ```bash
  git fetch origin
  git checkout main
  git merge origin/main
  ```
- Write a detailed PR description.
- Be responsive to feedback during the review process
- We will review it in a couple of days usually, please do not try to mention maintainers or otherwise annoy/pester us.

---

## Community Support

If you have questions, need guidance, or want to discuss contributions:

- Join our [Discord server](https://administer.notpyx.me/to/discord).
- Post on our [Discussion board](https://github.com/administer-org/issues/discussions).
  
---

## License

By contributing, you agree that your contributions will be licensed under the same license as the project (generally GNU AGPL 3.0). Refer to the [LICENSE](./LICENSE) file in the repository for details.

---

We're excited to collaborate with you! Thanks for contributing to Administer.
