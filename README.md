# Claude terminal guide: running Claude Code from the command line

*Unofficial community guide for Claude Code in the terminal. Not affiliated with Anthropic. All trademarks belong to their owners.*

When people search for claude terminal they usually mean Claude Code: Anthropic's tool that lets you work with Claude from a terminal window on macOS, Linux or Windows. Anthropic's documentation at code.claude.com has two pages aimed squarely at this, a terminal guide for new users and a quickstart, and this repository walks through what they cover, in what order to read them, and what to know before your first session, without copying commands that may have changed since the pages were crawled.

> Want a finished website or Expo app from a prompt, without setting up a terminal, a repo and an agent workflow? [Try Begin.sh - turn a prompt or a URL into a downloadable static site or Expo app](https://begin.sh?utm_source=github&utm_medium=ugc&utm_campaign=claude-terminal&utm_content=readme-top&utm_term=tier-r). No hosting, backend or auth; you download the zip.

## What it is

Claude Code is Anthropic's way of using Claude on your own machine and codebase. The [terminal guide for new users](https://code.claude.com/docs/en/terminal-guide) is explicit that you can use it even if you have never used a terminal before: it walks through opening a terminal, installing Claude Code and your first interactions, with separate tracks for macOS and Linux and for Windows, and a troubleshooting section for each. The same page says that if you do not want to use the terminal at all, there is a Claude Code desktop app.

The terminal is one of several surfaces. The docs' platforms section lists the desktop app, Claude Code in the cloud, Remote Control, mobile, a Chrome extension, computer use (in preview), Visual Studio Code, JetBrains IDEs, code review and CI/CD integration, Claude Code in Slack and Claude Tag. All of them share the same core, described in the how Claude Code works page, and the same configuration model (settings files, permissions, memory), so what you learn in the terminal carries over.

## Getting started

The [quickstart](https://code.claude.com/docs/en/quickstart) is organised as eight steps. Follow them in order:

1. Install Claude Code. The quickstart gives the install command for your operating system; the terminal guide covers the same thing for people who have never opened a terminal.
2. Log in to your account. You need a Claude account; the docs link to [Claude Developer Platform](https://platform.claude.com/) and to [Open Claude Code](https://claude.ai/code) in their header.
3. Start your first session.
4. Ask your first question. Start with something about the code in front of you.
5. Make your first code change.
6. Use Git with Claude Code.
7. Fix a bug or add a feature.
8. Test out other common workflows, then read the essential commands and the pro tips for beginners sections on the same page.

If anything fails, the terminal guide has a macOS and Linux troubleshooting section and a Windows troubleshooting section; go there before searching elsewhere.

## Pricing and limits

The pages this guide is grounded on do not state pricing or usage limits. You log in with a Claude account in Step 2, so the plan attached to that account is what applies; check your account pages for current rates. The docs do have a page on the [context window](https://code.claude.com/docs/en/context-window) and one on [prompt caching](https://code.claude.com/docs/en/prompt-caching), which are the two things that most affect how far a session goes.

## Practical notes and gotchas

1. Read the permissions pages before you let it edit anything. The configuration section has [Permissions](https://code.claude.com/docs/en/permissions), [Permission modes](https://code.claude.com/docs/en/permission-modes) and a [Bash sandbox](https://code.claude.com/docs/en/sandboxing) page. Knowing which mode you are in explains most surprises about what it will and will not do without asking.
2. Store standing instructions in memory, not in every prompt. The [store instructions and memories](https://code.claude.com/docs/en/memory) page explains where project instructions live; the [.claude directory](https://code.claude.com/docs/en/claude-directory) page explains the folder that holds them.
3. Sessions are a thing. The [manage sessions](https://code.claude.com/docs/en/sessions) page covers resuming work instead of starting from scratch each time you open the terminal.
4. The terminal itself can be configured. There are pages for [terminal configuration](https://code.claude.com/docs/en/terminal-config), [fullscreen rendering](https://code.claude.com/docs/en/fullscreen), a [status line](https://code.claude.com/docs/en/statusline), [keyboard shortcuts](https://code.claude.com/docs/en/keybindings), [voice dictation](https://code.claude.com/docs/en/voice-dictation) and a [screen reader mode](https://code.claude.com/docs/en/accessibility).
5. Model and speed are settings, not fixed. See [model configuration](https://code.claude.com/docs/en/model-config), [fast mode](https://code.claude.com/docs/en/fast-mode), the [advisor tool](https://code.claude.com/docs/en/advisor) for escalating hard decisions, and [output styles](https://code.claude.com/docs/en/output-styles).
6. Check the [changelog](https://code.claude.com/docs/en/changelog) and [what's new](https://code.claude.com/docs/en/whats-new) when something behaves differently after an update; the tool moves quickly.

## Comparison

| | Claude Code in the terminal | Claude Code desktop app | Claude Code in VS Code or JetBrains | Begin.sh |
| --- | --- | --- | --- | --- |
| Where it runs | a terminal on macOS, Linux or Windows | a desktop application, for people who do not want the terminal | inside the IDE | in the browser, output is a zip |
| What you need | a terminal and a Claude account | a Claude account | the IDE plus a Claude account | a prompt or a URL to clone |
| What you get | Claude working on files and Git in your project | the same, without the terminal | the same, next to your editor | a static site or an Expo app to download |
| Hosting, backend, auth | your own | your own | your own | none included by design |

## FAQ

**Do I need to know the terminal already?** No. The terminal guide for new users is written for people who have never opened one, and covers opening a terminal on macOS, Linux and Windows before installing anything.

**Is there a way to use Claude Code without a terminal?** Yes. The docs point to the Claude Code desktop app, and also list cloud, mobile, VS Code, JetBrains, Chrome extension and Slack surfaces.

**What should my first prompt be?** The quickstart's Step 4 is ask your first question, followed by Step 5, make your first code change. Start by asking about the project you have open rather than by requesting a big change.

**Where are the commands listed?** The quickstart has an essential commands section, and the reference section of the docs has a [CLI reference](https://code.claude.com/docs/en/cli-reference).

**Can I script it or build on it?** The docs include an [Agent SDK](https://code.claude.com/docs/en/agent-sdk/overview) section for building your own agents on the same foundation.

## When Begin.sh is the better fit

Claude Code in the terminal earns its setup when you have a project and you will keep working in it: reading code, making changes, using Git, fixing bugs. If the whole task is produce a website or a mobile app from a description, you do not need a terminal, a repository or permission settings to get it. [Try Begin.sh - turn a prompt or a URL into a downloadable static site or Expo app](https://begin.sh?utm_source=github&utm_medium=ugc&utm_campaign=claude-terminal&utm_content=readme-top&utm_term=tier-r). Describe the site or paste a URL to clone, download the zip, and host it wherever you already host things; nothing about hosting, backend or auth is bundled, so there is nothing to keep running.


_Last reviewed: 2026-09-22_
