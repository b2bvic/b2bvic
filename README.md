# Victor Valentine Romo: agent oversight, owned records, and SEO checks

These repositories come from a working setup that runs Claude Code and Codex CLI on hosted models for a small search consultancy.
Each tool solves one problem that setup hit: agents that forget the business, agent work nobody can audit, and pages nobody checked.

[Project page](https://scalewithsearch.com/code/b2bvic) · Victor Valentine Romo · [Scale With Search](https://scalewithsearch.com)

## Start here

| Repository | What it does |
| --- | --- |
| [agent-oversight](https://github.com/b2bvic/agent-oversight) | Checks agent work from outside the agent: response rules, process status, review receipts for parallel coding agents, and dry-run gates before API writes. |
| [owned-record](https://github.com/b2bvic/owned-record) | Keeps agent context and session history in Markdown and SQLite files you control, so a change of model or vendor does not erase what the agents knew. |
| [seo-checks](https://github.com/b2bvic/seo-checks) | Runs 20 page checks from one command: `seo-checks robots`, `seo-checks redirects`, `seo-checks schema-product`, and more. |
| [declip](https://github.com/b2bvic/declip) | Removes filler words from talking-head video with local Whisper transcription and ffmpeg on Apple Silicon. You preview each cut before it runs. |

## Also here

| Repository | What it does |
| --- | --- |
| [ops-scripts](https://github.com/b2bvic/ops-scripts) | Small operator scripts: Telegram alerts, Linux host checks, a macOS Messages export, an X bookmark import, and an X posting queue. |
| [vault-crawl](https://github.com/b2bvic/vault-crawl) | A Rust retrieval core that stores fetched pages with provenance, content-addressed blobs, and SQLite search. |

## Site sources

[polytraffic](https://github.com/b2bvic/polytraffic), [creatinepedia](https://github.com/b2bvic/creatinepedia), [ivibecodeditforyou](https://github.com/b2bvic/ivibecodeditforyou), and [AIPayPerCrawl](https://github.com/b2bvic/AIPayPerCrawl) hold the source for content sites built on the same stack.

## Moved repositories

The earlier single-tool repositories are archived. Each archived README names its new folder. For example, `observer-daemon` is now `agent-oversight/components/observer-daemon`, and `sitemap-check` is now `seo-checks sitemap`.

## Provenance

This README was written with model assistance from the current repository files. Each repository README is the authority for its tool's setup and limits.
