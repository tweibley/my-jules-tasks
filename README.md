# My jules Tasks

This repository contains my personal set of tasks for [jules](https://jules.google/docs), an AI agent framework. These tasks are primarily focused on maintaining and improving my Ruby projects.

## Purpose

The goal of this repository is to provide a collection of specialized agents (implemented as jules tasks) that can be scheduled to run against my Ruby codebases. These agents are designed for **Ruby gems, libraries, and applications** (framework-agnostic, not Rails-specific). Each agent has a specific focus area, such as architecture, documentation, performance, or security.

## Repository Structure

- `scheduled/`: Contains the task definitions for various scheduled jules agents.
  - [`atlas.md`](scheduled/atlas.md): Architecture Agent 🗺️ - Focuses on system design and organization.
  - [`beacon.md`](scheduled/beacon.md): Testing & Reliability Agent 🚦 - Focuses on test coverage and edge cases.
  - [`bolt.md`](scheduled/bolt.md): (Built-in, Modified) Performance Agent ⚡ - Focuses on optimization and efficiency.
  - [`compass.md`](scheduled/compass.md): Onboarding & Contribution Agent 🧭 - Focuses on developer experience and setup.
  - [`palette.md`](scheduled/palette.md): (Built-in, Modified) Developer Experience Agent 🎨 - Focuses on API ergonomics and UX.
  - [`scout.md`](scheduled/scout.md): Code Quality Agent 🔭 - Focuses on maintainability and code smells.
  - [`scribe.md`](scheduled/scribe.md): Documentation Agent 📝 - Focuses on clear explanations and discoverability.
  - [`sentinel.md`](scheduled/sentinel.md): (Built-in, Modified) Security Agent 🛡️ - Focuses on vulnerability detection and security best practices.

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
