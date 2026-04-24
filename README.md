<p align="center">
  <img src="assets/hob-icon.svg" alt="hob logo" width="128">
</p>

# hob

`hob` is the independent workspace for coding agents.

It gives developers one tiled surface for the agent tools they already use: Claude Code, Codex, OpenCode, terminals, file viewers, diffs, and task context side by side. hob is the workspace layer, not the inference provider, so model choice, subscriptions, and workflow stay under your control.

This repository is the public place to track feedback for hob.

Use this repository to:

- Request features or workflow improvements for agent workspaces
- Report bugs in released builds
- Ask usage questions that could help other users
- Track public-facing product issues

Please do not report security vulnerabilities in public issues. See [SECURITY.md](SECURITY.md) for how to report security concerns.

## Before Opening An Issue

- Search existing issues first to avoid duplicates.
- Include the version or commit you are using when reporting a bug.
- Include your operating system and whether you are using desktop, headless, roam, relay, or gateway mode when relevant.
- For UI bugs, screenshots or short screen recordings are helpful.
- For agent or terminal bugs, include the relevant log excerpt if you can.

## Useful Logs

If an issue is hard to reproduce or diagnose, run `hob` with `--debug` and attach the relevant log excerpt. Debug mode generates extremely verbose logs that are useful for agents and maintainers to pinpoint issues.

Debug logs are written under the `logs` directory inside hob's app config directory:

| OS | Log directory |
| --- | --- |
| Linux | `~/.config/SmartAppsCo/hob/logs/` |
| macOS | `~/Library/Application Support/SmartAppsCo/hob/logs/` |
| Windows | `%AppData%\SmartAppsCo\hob\logs\` |

Logs are grouped by project in a normalized project folder. For project-specific logs, look for the newest `hob_YYYYMMDD_HHMMSS_mmm_pidNNN.log` file under the matching project folder.

## Scope

This repository is for public coordination. It is not an open-source software repository, and it is not intended to mirror the full source repository or development history.

All rights are reserved by SmartAppsCo LLC. See [LICENSE.md](LICENSE.md).
