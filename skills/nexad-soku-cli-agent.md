# Use Soku CLI With an AI Agent

You are helping a user connect Claude Code, Codex, Cursor, or another
shell-based AI agent to Soku. Follow the steps in order. Setup is complete only
after you produce the first useful task result; installation alone is not
activation. Never ask the user for third-party provider API keys.

## Goal

Install or update Soku CLI, sign in, select the user's remote Soku workspace,
install only the business skills required for the task, verify the available
surfaces, and complete a concrete read-only task. Stop for browser approval,
ambiguous workspace selection, or a review-gated write.

## 1. Check prerequisites

```bash
node --version
npm --version
```

Node.js must be 20 or newer. If Node.js is missing or too old, ask the user to
install Node.js 20+ first.

## 2. Install or update the CLI

```bash
npm i -g @soku-ai/cli
soku --version
soku update status
```

If npm says `@soku-ai/cli` is not found, report that the official package is
unavailable. Do not invent an unofficial package name.

## 3. Sign in

For a shell/container agent, prefix every login call, including the resume
command, with `SOKU_NO_KEYCHAIN=1`. This avoids an indefinite OS-keychain or
D-Bus wait and stores the token in `~/.soku/credentials.json` with mode 0600.

Start the non-blocking device flow:

```bash
SOKU_NO_KEYCHAIN=1 soku auth login --no-wait
```

Show the returned verification URL and user code, then stop and wait for the
user to approve in the browser. Resume with the exact `next` command returned
by the CLI, prefixed the same way, usually:

```bash
SOKU_NO_KEYCHAIN=1 soku auth login --device-code <device_code>
```

For an interactive human terminal, this is also acceptable:

```bash
soku auth login
```

A default login reaches the current CLI surface. Do not add a resource bundle
flag. Review-gated ads mutations create a pending review for a human to approve.
Direct-write surfaces such as SEO Hosting require explicit user confirmation in
the task prompt or agent harness before execution.

## 4. Select a workspace

Do not infer the Soku workspace from the local folder. Use the remote org and
brand the user wants the agent to operate on.

```bash
soku workspace status
soku workspace resolve <brand>
soku workspace use-brand <brand>
```

If there are multiple brand matches, show the candidates and ask the user which
one to use.

## 5. Install only the skills needed for the task

List the catalog, choose the narrowest relevant business skill, install it, and
verify the managed installation. Avoid installing the entire catalog unless the
user explicitly asks for it.

```bash
soku skill list
soku skill install <skill-slug> --global
soku skill status --global
soku skill list-installed --global
```

Installed business skills appear with a `soku-` prefix in agent skill
autocomplete. Invoke the installed skill for the user's concrete task.

## 6. Verify available surfaces

```bash
soku ads --help
soku ga4 --help
soku gsc --help
soku posthog --help
soku egress providers
soku seo-hosting status
```

If a command reports expired authentication, repeat login. If it reports no
workspace, repeat workspace selection. Read command help before using an
unfamiliar action or flag.

## 7. Produce the first useful result

A saved, read-only performance health check with the selected account, exact date window, evidence, and next actions — not merely a successful installation.

If the user has not specified a task, ask them to choose one connected account,
then run a read-only 30-day performance health check and save the findings. Do
not count package installation, login, or a help command as the completed task.

## What the agent can do

- Use typed `soku ads ...`, `soku ga4 ...`, `soku gsc ...`, and
  `soku posthog ...` commands for marketing and product analytics.
- Use focused `soku-*` business skills for audits, reports, research, content,
  creative workflows, and more.
- Use `soku egress -- curl ...` for covered third-party APIs with credentials
  injected server-side.
- Use `soku seo-hosting ...` to inspect, author, and publish pages when the
  user has approved the destination and public change.

## Rules

- Never print Soku tokens or ask the user to paste provider keys.
- Never infer a workspace when multiple matches exist.
- Never treat memory as live performance data; verify current claims with data
  commands.
- For review-gated writes, show the review ID and exact summary. A human must
  authorize the specific review before `soku review approve <id>` runs. Never
  allowlist or auto-approve that command.
- For SEO Hosting Cloudflare setup, never pass Cloudflare tokens as literal argv
  values. Use `--cf-token-env` or `--cf-token-stdin`.
