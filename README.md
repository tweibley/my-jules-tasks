# My jules Tasks

This repository contains my personal set of tasks for [jules](https://jules.google/docs), an AI agent framework. These tasks are primarily focused on maintaining and improving my Ruby projects.

## Purpose

The goal of this repository is to provide a collection of specialized agents (implemented as jules tasks) that can be scheduled to run against my Ruby codebases. These agents are designed for **Ruby gems, libraries, and applications** (framework-agnostic, not Rails-specific). Each agent has a specific focus area, such as architecture, documentation, performance, or security.

## Repository Structure

- `scheduled/`: Contains the task definitions for various scheduled jules agents.
  - `atlas.md`: Architecture Agent 🗺️ - Focuses on system design and organization.
  - `beacon.md`: Quality Agent 🚨 - Focuses on bug detection and code quality.
  - `bolt.md`: (Built-in, Modified) Performance Agent ⚡ - Focuses on optimization and efficiency.
  - `compass.md`: Direction Agent 🧭 - Focuses on alignment with project goals and standards.
  - `palette.md`: (Built-in, Modified) Style Agent 🎨 - Focuses on consistent formatting and idiomatic Ruby.
  - `scout.md`: Exploration Agent 🔍 - Focuses on discovering new opportunities and edge cases.
  - `scribe.md`: Documentation Agent 📝 - Focuses on clear explanations and discoverability.
  - `sentinel.md`: (Built-in, Modified) Security Agent 🛡️ - Focuses on vulnerability detection and security best practices.

## Usage

These tasks are designed to be used with jules. For more information on how to run and schedule these tasks, refer to the [jules documentation](https://jules.google/docs).

## Security

This repository includes a pre-commit hook to prevent accidentally committing sensitive data like passwords, API keys, or tokens.

### Setup

```bash
# Option 1: Configure git to use the .githooks directory
git config core.hooksPath .githooks

# Option 2: Copy the hook directly
cp .githooks/pre-commit .git/hooks/pre-commit
chmod +x .git/hooks/pre-commit
```

### What it detects

- API keys and tokens (AWS, GitHub, Google, Stripe, etc.)
- Passwords and secrets in configuration
- Private keys (RSA, SSH, EC, DSA, PGP)
- Bearer tokens and auth credentials

### Bypassing (use with caution)

If you encounter a false positive:
```bash
git commit --no-verify -m "Your message"
```

## Location

This repository is hosted at [github.com/tweibley/my-jules-tasks](https://github.com/tweibley/my-jules-tasks).
