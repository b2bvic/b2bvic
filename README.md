# Victor Valentine Romo: agent oversight, owned records, and SEO checks

Tools from a working setup that runs Claude Code and Codex CLI on hosted models for a small search consultancy.
Each repository fixes one problem that setup hit: agent sessions that start without the business context, agent work nobody can audit, video that needs cutting, and pages nobody checked before launch.

[Project page](https://scalewithsearch.com/code/b2bvic) · Victor Valentine Romo · [Scale With Search](https://scalewithsearch.com)

## Start here

| Repository | What it does | Try it |
| --- | --- | --- |
| [agent-oversight](https://github.com/b2bvic/agent-oversight) | Checks agent work from outside the agent: scores responses against your writing rules, lists running Claude and Codex sessions with recorded tokens, binds code review receipts to file hashes, and holds REST writes in dry-run until a human enables execution. | `python3 -m unittest discover -s tests -v` |
| [owned-record](https://github.com/b2bvic/owned-record) | Keeps domain context in Markdown and Claude Code and Codex transcripts in SQLite with full-text search, so a change of model or vendor leaves the record in place. Three opt-in hooks hand files and search results to Claude Code. | `bash examples/demo.sh` |
| [seo-checks](https://github.com/b2bvic/seo-checks) | Runs 20 SEO page checks from one command: `seo-checks robots`, `seo-checks redirects`, `seo-checks schema-product`, and 17 more, each with JSON output. | `seo-checks robots https://example.com` |
| [declip](https://github.com/b2bvic/declip) | Plans filler, silence, and retake cuts in local audio or video with Whisper transcription and ffmpeg. You accept or reject every cut on a local review page before it renders; the source file stays unchanged. Version 0.5.1 installs from the Git tag. | `uv tool install "declip[mac] @ git+https://github.com/b2bvic/declip@v0.5.1"` |

## Also here

| Repository | What it does |
| --- | --- |
| [ops-scripts](https://github.com/b2bvic/ops-scripts) | Five operator scripts: Telegram alerts, Linux host checks, a macOS Messages export, an X bookmark import, and an X posting queue. Each README states what it reads and what it writes. |
| [vault-crawl](https://github.com/b2bvic/vault-crawl) | A Rust retrieval core that stores fetched pages with provenance, content-addressed blobs, and SQLite search. |

## Site sources

[polytraffic](https://github.com/b2bvic/polytraffic), [creatinepedia](https://github.com/b2bvic/creatinepedia), [ivibecodeditforyou](https://github.com/b2bvic/ivibecodeditforyou), and [AIPayPerCrawl](https://github.com/b2bvic/AIPayPerCrawl) hold the Markdown and build scripts for content sites on the same stack.

## Moved repositories

The 39 earlier single-tool repositories are archived, and each archived README names its new folder. `observer-daemon` is now `agent-oversight/components/observer-daemon`; `sitemap-check` is now `seo-checks sitemap`; `session-ledger` is now `owned-record/components/session-ledger`.

## Provenance

This README was written with model assistance from the current repository files. Each repository README is the authority for its tool's setup, data boundaries, and limits.
