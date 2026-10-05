# Agent orchestration and owned memory examples: b2bvic

This profile collects agent orchestration and owned memory examples for team leads who use hosted models.
Use these patterns when you must repeat business context or cannot recover an agent's work history.

[Project page](https://scalewithsearch.com/code/b2bvic) · Victor Valentine Romo

## Agent orchestration

Start with [agent-oversight](https://github.com/b2bvic/agent-oversight), the overview of independent tools for inspecting agent work.
These are patterns a team can adopt with Claude Code and Codex CLI, subject to each tool's integration limits.

| Repository | What the files demonstrate |
| --- | --- |
| [session-ledger](https://github.com/b2bvic/session-ledger) | Archive Claude Code and Codex session records in SQLite, then export shared records as JSON. |
| [safe-api](https://github.com/b2bvic/safe-api) | Preview REST writes with dry runs, endpoint checks, duplicate callbacks, and JSONL receipts. |
| [observer-daemon](https://github.com/b2bvic/observer-daemon) | Check response text against configured writing rules and record corrections. |

## Owned memory

Start with [owned-record](https://github.com/b2bvic/owned-record), the reference for domain context and activity logs in Markdown.
Use [pretool-memory](https://github.com/b2bvic/pretool-memory) for a Claude Code hook that retrieves local knowledge before selected tools.

Keep an owned record. Prepare relevant context from that record. Keep human judgment at the decision and side-effect boundary.
Markdown files and exported session JSON provide portable AI agent records. Client hooks still need their own integrations.

## Install

Install each tool from its repository README. This profile contains documentation.
The quick start requires `curl`.

## Quick start

Use an empty directory for these commands. Fetch both hub READMEs into that directory:

```bash
curl -fsSL https://raw.githubusercontent.com/b2bvic/agent-oversight/main/README.md -o agent-oversight.md
curl -fsSL https://raw.githubusercontent.com/b2bvic/owned-record/main/README.md -o owned-record.md
wc -l agent-oversight.md owned-record.md
```

Read both files before installing a tool. The commands download documentation; they do not install hooks.

## How it works

Claude Code workflow patterns include context pointers and optional retrieval hooks.
Codex CLI workflow patterns include transcript capture through Session Ledger.
The oversight hub explains how to inspect records and evaluate changes.

## Limits

- The public examples come from a single-operator work record. They do not establish team deployments or customer outcomes.
- The tools run independently. The overview does not ship an integrated orchestrator or a shared approval service.
- A retrieved record can contain an incorrect statement. A writing score does not establish factual accuracy.
- Enforce human approval where software sends, publishes, deletes, spends, or changes production state.
- Data portability does not make a Claude Code hook compatible with another client.

The [source evidence](EVIDENCE.md) identifies the inspected revisions and implementation boundaries.

## Related repositories

- [agent-oversight](https://github.com/b2bvic/agent-oversight): orchestration overview and evaluation guidance.
- [owned-record](https://github.com/b2bvic/owned-record): Markdown memory overview and context routing.

## Work with me

See [Scale With Search](https://scalewithsearch.com/work) for current scope and terms.

## Provenance

This profile README was written from the current repository files, with model assistance. Each repository README is the authority for its tool's limits.
