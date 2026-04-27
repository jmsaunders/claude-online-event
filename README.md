# online-event

A Claude Code skill for the [Drupal AI Initiative](https://www.drupal.org/project/ai_initiative) that generates structured GitLab issue files for webinars and podcast episodes.

## Background

The Drupal AI Initiative runs a recurring programme of webinars and podcast episodes. Each one involves the same core work: planning, content, production, promotion, and post-event follow-up. Without a consistent structure, issues get created ad hoc, steps get missed, and contributors have to reinvent the wheel every time.

This skill solves that. When you invoke `/online-event` in Claude Code, it asks you a few questions about the event and generates a full folder of issue files ready to copy into GitLab. Every file follows the same structure and includes a tracker block and AI usage checkboxes aligned with the Initiative's standards.

## Requirements

- [Claude Code](https://claude.ai/code)

## Installation

Clone this repository into your Claude Code skills directory:

```bash
git clone https://github.com/jmsaunders/claude-online-event.git ~/.claude/skills/online-event
```

Restart Claude Code. The `/online-event` command will be available immediately.

## Usage

Run `/online-event` from any Claude Code session. The skill will ask:

- Webinar or podcast episode?
- Guest or speaker details
- Topic and target date
- Source material URLs
- Hosts
- Social media contacts

It will propose a folder name for your confirmation, then generate the full issue structure in your current working directory.

## Sharing with your team

Anyone using Claude Code can install this skill using the same `git clone` command above. If you want the skill available to everyone working in a specific repository, copy `SKILL.md` into `.claude/skills/online-event/SKILL.md` inside that repo — no separate install required.
