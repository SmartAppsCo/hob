<p align="center">
  <img src="assets/hob-icon.svg" alt="hob logo" width="128">
</p>

# hob

**Work with your agents, not just through them.**

hob is the independent workspace where people and agents work together. It
supports every way of working with agents:

- **Beside you.** The agent works in view. It operates web pages while you
  watch, points at details, and hands a step back to you. You mark up pages,
  images, PDFs, and spreadsheets, and you can take control at any time.
- **In parallel.** Run several agents on one project, on the same backend or
  on different backends. Give each agent its own task, let agents review
  each other's work, and send messages between them.
- **In the background.** Send a task away and come back to the result. Queue
  or schedule messages, and keep agents working on a headless Host while you
  are away.
- **As automations.** Save useful steps as a skill or an automation. Run it on
  demand, from an agent, from the CLI, or on a schedule. hob keeps a record of
  each run.

Whichever way the work runs, it stays in one project with its record: web pages,
documents, spreadsheets (beta), data, and code, beside the conversations and
runs that changed them.

**Keep the work. Change what runs it.** Use Claude Code, Codex, OpenCode, or
Grok Build with your own provider accounts. hob sells workspace software and
stays out of the inference path.

[Download hob](https://hob.dev/download) · [Documentation](https://hob.dev/docs) · [Pricing](https://hob.dev/pricing)

## Send feedback from the app

The fastest way to reach us is from inside hob. Select the smiley face in the
top-right corner of the window.

- **Feedback:** Send praise, ideas, or anything else. A person reads every note.
- **Report a problem:** Describe what happened and what you expected. You can
  paste screenshots, and you can choose to attach system information and the
  debug logs for the related runs. If the problem needs more detail, select
  **Restart in debug**, reproduce the problem, and then send the report.

You choose what to attach. hob encrypts the report before it sends it. Add an
email address if you want a reply.

## About this repository

This repository is the public place to give feedback about hob. Use it to:

- Report bugs in released builds.
- Request features or workflow improvements.
- Ask usage questions that can help other users.
- Track public product issues.

Do not report security vulnerabilities in public issues. See
[SECURITY.md](SECURITY.md) for the procedure.

## Before you open an issue

1. Search the existing issues for duplicates.
2. Give the hob version that you use. Say if it is a stable or a beta build.
3. Give your operating system.
4. Say how you use hob, if it is related: desktop, headless, browser IDE, hob
   mobile, or relay.
5. For UI bugs, attach a screenshot or a short screen recording.
6. For agent or terminal bugs, attach the related log lines.

If you can open hob, use **Report a problem** in the app first. It collects
most of this information for you.

## Debug logs

If a problem is difficult to reproduce, start hob with `--debug` and attach the
related lines from the log. Debug logs are very detailed. They help agents and
maintainers find the cause.

Beta builds write debug logs by default.

hob writes debug logs to the `logs` directory in its app config directory:

| OS | Log directory |
| --- | --- |
| Linux | `~/.config/SmartAppsCo/hob/logs/` |
| macOS | `~/Library/Application Support/SmartAppsCo/hob/logs/` |
| Windows | `%AppData%\SmartAppsCo\hob\logs\` |

Each project has its own folder in this directory. Use the newest
`hob_YYYYMMDD_HHMMSS_mmm_pid<pid>_run<runID>.log` file in the project folder.
Other files from the same launch have the same `_run<runID>` suffix.

Logs can contain file paths, project names, and parts of conversations. Remove
private data before you attach them.

## Scope

This repository is for public coordination. It is not an open-source
repository. It does not mirror the source code or the development history.

All rights are reserved by SmartAppsCo LLC. See [LICENSE.md](LICENSE.md).
