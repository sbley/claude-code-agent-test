# claude-code-agent-test

A test repository for exploring and demonstrating the capabilities of [Claude Code](https://claude.ai/code) through GitHub Actions workflows.

## Overview

This repository serves as a testing ground for Claude Code automation, featuring several workflow integrations that showcase how AI can assist with development tasks.

## Features

### 🤖 Claude Code Integration
The repository includes three GitHub Actions workflows that leverage Claude Code:

- **Interactive Claude Assistant** (`.github/workflows/claude.yml`)
  Responds to `@claude` mentions in issues, pull requests, and comments to perform various tasks like code reviews, bug fixes, and feature implementations.

- **Automated Code Review** (`.github/workflows/claude-code-review.yml`)
  Automatically reviews pull requests for code quality, potential bugs, performance issues, security concerns, and test coverage.

- **AI Model Release Monitor** (`.github/workflows/ai-model-release-monitor.yml`)
  Runs daily to monitor and track new AI model releases from major providers (OpenAI, Anthropic, Google, Meta, Alibaba, xAI, Mistral, Cohere), creating GitHub issues for significant releases.

## Getting Started

### Prerequisites

To use the Claude Code workflows in this repository, you need:

1. A GitHub repository with GitHub Actions enabled
2. A Claude Code OAuth token configured as `CLAUDE_CODE_OAUTH_TOKEN` in repository secrets

### Usage

**Invoke Claude on Issues or Pull Requests:**
Simply mention `@claude` in an issue, PR comment, or review to get AI assistance. Examples:
- `@claude review this PR`
- `@claude fix the bug in authentication.ts`
- `@claude help me implement dark mode`

**Automatic Code Reviews:**
Code reviews are automatically triggered when PRs are opened or updated (can be customized to filter by author or file paths).

**AI Model Monitoring:**
The monitor runs automatically once daily at 8 AM CET, or can be triggered manually via workflow dispatch.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## Author

Stefan Bley

## Acknowledgments

Built using [Claude Code](https://claude.ai/code) by Anthropic.
