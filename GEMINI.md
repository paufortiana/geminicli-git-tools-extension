# Project Overview

This project is a Gemini CLI extension named "git-tools," designed to enhance the user's Git workflow. The extension integrates directly with the Gemini CLI to provide helpful Git-related commands.

The core features of this extension are the `/git-commit:write` and `/git-commit:amend` commands, which analyze the user's staged code changes and suggests a professional, high-quality commit message. The generated message is designed to adhere to the **Conventional Commits specification**, promoting clear, concise, and standardized version control history.

The primary technologies and conventions used are:

- **Gemini CLI Extensions**: The project is structured as an extension for the Gemini CLI.
- **TOML**: Command definitions and prompts are configured using TOML files.
- **Conventional Commits**: The logic for generating commit messages strictly follows the Conventional Commits 1.0.0 specification.

## Building and Running

There is no explicit build step required for this extension. It is intended to be installed and run directly through the Gemini CLI.

**Installation:**
To install the extension, run the following command in your terminal:

```bash
gemini extensions install <repository_url>
```

**Running the Command:**
Once installed, the primary command can be invoked within the Gemini CLI:

```bash
/git-commit:write
```

This command will analyze the staged Git diff and generate a suggested commit message.

## Development Conventions

The main development convention for this project is the strict adherence to the **Conventional Commits specification**. Any contributions or modifications, especially to the commit message generation logic, should follow these guidelines.

**Commit Message Structure:**
The expected commit message format is:

```bash
type(scope): imperative, short description

[optional body]

[optional footer]
```

- **Types**: `feat`, `fix`, `docs`, `style`, `refactor`, `perf`, `test`, `chore`, `ci`, `revert`.
- **Subject Line**: Must be 50 characters or less and written in the imperative mood.
- **Body/Footer**: Optional, used for providing additional context, referencing issues, or noting breaking changes.
