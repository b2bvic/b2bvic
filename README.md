# Victor Valentine Romo

I get businesses found in Google and AI answers, then build the system they own.

[Scale With Search](https://scalewithsearch.com) · [How it works](https://scalewithsearch.com/how-it-works) · [All tools](https://scalewithsearch.com/code/) · [X](https://x.com/scalewithsearch)

## How I work

Search moved. The job did not. In 2013 the question was how a business ranked in Google. Now the buyer asks an AI and gets one answer. Either way, the engine needs a current record of what a business does, where, for whom, and at what price. Most businesses do not have one. Their facts live in old chats, a stale site, and listings that disagree. The answer repeats whichever version it found.

Scale With Search fixes the record and the pages the engines read. Four rules hold on every job:

- **One current record.** Every fact has one current version, in a file the business owns. The pages, the listings, and any AI pointed at the record read from the same place.
- **Fix the source before the symptom.** Rankings and AI answers follow what the engines can read. A report describes the problem. It does not fix it.
- **Approval at the action boundary.** Sends, publishing, purchases, deletions, and live account changes wait for a named person to approve them.
- **People at both ends.** A person gives the direction. A person checks the result before anything leaves the business.

The price is fixed and written before money moves. The method is public. The files stay with the client. There is no account manager: I write the scope, AI agents draft and test in parallel, and I review every output before it ships.

The tools below are that method, in code. Each one came out of my own work and fixes one problem that work hit.

## Search tools

| Repository | What it does | Try it |
| --- | --- | --- |
| [content-brief-dfs](https://github.com/b2bvic/content-brief-dfs) | Surfer- and Clearscope-style content briefs, computed from the DataForSEO API. Measures the ranking pages: term ranges, entities, topic coverage, and the searches ChatGPT runs for the keyword. Marks the questions no page answers, and scores a draft. About $0.05 a keyword. | `content-brief brief 'your keyword' --llm-fanout --dry-run` |
| [seo-checks](https://github.com/b2bvic/seo-checks) | Twenty SEO page checks from one command: `seo-checks robots`, `seo-checks redirects`, `seo-checks schema-product`, and 17 more, each with JSON output. | `seo-checks robots https://example.com` |

## Agent tools

| Repository | What it does | Try it |
| --- | --- | --- |
| [agent-oversight](https://github.com/b2bvic/agent-oversight) | Checks agent work from outside the agent. Scores responses against your writing rules, lists running Claude Code and Codex sessions with their tokens, binds code review receipts to file hashes, and holds REST writes in dry-run until a person enables them. | `python3 -m unittest discover -s tests -v` |
| [owned-record](https://github.com/b2bvic/owned-record) | Keeps business context in Markdown and Claude Code and Codex transcripts in SQLite with full-text search. Change the model or the vendor; the record stays. | `bash examples/demo.sh` |
| [vault-crawl](https://github.com/b2bvic/vault-crawl) | A Rust retrieval core: fetched pages stored with provenance, content-addressed blobs, and SQLite search. | |

## Media and operations

| Repository | What it does |
| --- | --- |
| [declip](https://github.com/b2bvic/declip) | Plans filler, silence, and retake cuts in local audio or video with Whisper and ffmpeg. You accept or reject every cut on a local review page before it renders. The source file stays unchanged. |
| [ops-scripts](https://github.com/b2bvic/ops-scripts) | Five operator scripts: Telegram alerts, Linux host checks, a macOS Messages export, an X bookmark import, and an X posting queue. Each README states what it reads and writes. |

## Site sources

[polytraffic](https://github.com/b2bvic/polytraffic), [creatinepedia](https://github.com/b2bvic/creatinepedia), [ivibecodeditforyou](https://github.com/b2bvic/ivibecodeditforyou), and [AIPayPerCrawl](https://github.com/b2bvic/AIPayPerCrawl) hold the Markdown and build scripts for content sites on the same stack.

## Archived

The 39 earlier single-tool repositories are archived. Each archived README names its new home: `observer-daemon` is now in `agent-oversight`, `sitemap-check` is `seo-checks sitemap`, and `session-ledger` is in `owned-record`.

Each repository README is the authority on its setup, data boundaries, and limits. [EVIDENCE.md](EVIDENCE.md) links the source lines behind the claims on this page.
