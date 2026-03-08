# PR Comment Watcher

Sends a Slack notification whenever a PR or issue comment is **edited** (not just created).

Uses a GitHub Action triggered on `issue_comment: [edited]` to detect changes and posts the diff to Slack via incoming webhook.

## Setup

1. Add your Slack webhook URL as a repository secret named `SLACK_WEBHOOK_URL`
2. That's it — edits to any comment on PRs or issues will trigger a Slack notification

## What you get in Slack

- Who edited the comment
- Which PR/issue it's on
- What changed (before → after)
- Direct link to the comment
