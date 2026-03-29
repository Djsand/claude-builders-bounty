# claude-review — PR Review Agent

> A Claude Code sub-agent that fetches a GitHub PR diff and returns a structured Markdown code review.

Fixes [#4](https://github.com/claude-builders-bounty/claude-builders-bounty/issues/4) — AGENT: Claude Code sub-agent that reviews a PR and posts a structured comment.

## Features

- 🔍 Fetches PR diffs via the GitHub API (handles diffs up to 80 KB; truncates larger ones gracefully)
- 🤖 Analyzes diffs using Claude (`claude-opus-4-5`)
- 📋 Returns structured Markdown with **Summary**, **Risks**, **Improvement Suggestions**, and **Confidence Score**
- 💾 Optionally saves output to a file with `--output`
- 🔄 Includes a GitHub Action for automated PR review comments

## Setup