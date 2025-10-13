# Gemini CLI Git Tools Extension

The Git Tools extension is an open-source Gemini CLI extension, built to enhance your repository's git workflow. The extension adds new commands to Gemini CLI that help with git.

## Installation

Install the Git Tools extension by running the following command from your terminal *(requires Gemini CLI v0.4.0 or newer)*:

```bash
gemini extensions install https://github.com/paufortiana/geminicli-git-tools-extension
```

If you do not yet have Gemini CLI installed, or if the installed version is older than 0.4.0, see
[Gemini CLI installation instructions](https://github.com/google-gemini/gemini-cli?tab=readme-ov-file#-installation).

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

## Resources

- [Gemini CLI extensions](https://github.com/google-gemini/gemini-cli/blob/main/docs/extensions/index.md): Documentation about using extensions in Gemini CLI
- [Blog post](https://blog.google/technology/developers/gemini-cli-extensions/): Announcement of Gemini CLI Extensions
- [GitHub issues](https://github.com/paufortiana/geminicli-git-tools-extension/issues): Report bugs or request features

## Legal

- License: [Apache License 2.0](https://github.com/paufortiana/geminicli-git-tools-extension/blob/main/LICENSE)
