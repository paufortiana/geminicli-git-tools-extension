# Gemini CLI Git Tools Extension

The Git Tools extension is an open-source Gemini CLI extension, built to enhance your repository's git workflow. The extension adds new commands to Gemini CLI that help with git.

## Installation

Install the Git Tools extension by running the following command from your terminal *(requires Gemini CLI v0.4.0 or newer)*:

```bash
gemini extensions install https://github.com/paufortiana/geminicli-git-tools-extension
```

If you do not yet have Gemini CLI installed, or if the installed version is older than 0.4.0, see
[Gemini CLI installation instructions](https://github.com/google-gemini/gemini-cli?tab=readme-ov-file#-installation).

## A Note on Gemini CLI's Evolution

The Gemini CLI is experiencing incredibly rapid development, with frequent updates introducing powerful new features. While this extension aims to enhance your Git workflow, it is important to acknowledge that the Gemini CLI's own rapid evolution may quickly integrate or even supersede some of the functionalities offered here.

## Commands

This extension provides the following commands:

### `/git-commit:write`

Analyzes your staged git changes and suggests a professional, high-quality commit message that adheres to the Conventional Commits specification.

**Usage:**

1. Stage your changes using `git add`.
2. Run the command in your Gemini CLI terminal.
3. The extension will return a suggested commit message.

### `/git-commit:amend`

Analyzes your staged git changes and suggests a professional, high-quality commit message to amend the previous commit, that adheres to the Conventional Commits specification.

**Usage:**

1. Stage your changes using `git add`.
2. Run the command in your Gemini CLI terminal.
3. The extension will return a suggested commit message to amend the previous commit.

### `/git-pr:draft`

Generates a Pull Request title and description based on your branch's changes against a target branch.

**Usage:**

1. Ensure you are on your feature branch.
2. Run the command in your Gemini CLI terminal.
3. The extension will analyze your changes and generate a draft PR description.

## Roadmap

I would like to enhance the Git Tools extension for the Gemini CLI. Here's a look at what's planned:

### Git Rebase Commands

I plan to introduce new commands under a `/git-rebase` namespace to streamline your rebasing workflows. These commands will aim to:

* **Interactive Rebase Assistance**: Provide intelligent suggestions and automation for interactive rebasing, making it easier to squash, fixup, and reorder commits.
* **Conflict Resolution Guidance**: Offer guided steps and context-aware suggestions to resolve merge conflicts during a rebase operation.
* **Conventional Commits Integration**: Ensure that any rebase operations that modify commit messages can leverage the Conventional Commits specification for consistency.

I welcome contributions and feedback on these upcoming features!

## Resources

* [Gemini CLI extensions](https://github.com/google-gemini/gemini-cli/blob/main/docs/extensions/index.md): Documentation about using extensions in Gemini CLI
* [Blog post](https://blog.google/technology/developers/gemini-cli-extensions/): Announcement of Gemini CLI Extensions
* [GitHub issues](https://github.com/paufortiana/geminicli-git-tools-extension/issues): Report bugs or request features

## Legal

* License: [Apache License 2.0](https://github.com/paufortiana/geminicli-git-tools-extension/blob/main/LICENSE)
