# Victor Valentine Romo

SEO consultant. I get businesses found in Google and AI answers, then build the system they own.

[Scale With Search](https://scalewithsearch.com) · [Send your brief](https://scalewithsearch.com/work#send-your-brief) · [How it works](https://scalewithsearch.com/how-it-works) · [Proof](https://scalewithsearch.com/proof) · [All tools](https://scalewithsearch.com/code/) · [X](https://x.com/scalewithsearch)

## Find, fix, own

Buyers ask Google who to call. Now they ask AI too. The question has not changed since I started in search in 2013: who does this, near me, for what price. What changed is who answers.

1. **Find** what Google and AI say about the business now, and which pages they pull it from.
2. **Fix** the pages and the facts they pull from, with one current version of each fact.
3. **Own** the record. It goes into readable files the business keeps, and those files become its AI system.

## Two jobs

**Website and search.** For small service businesses that want the fix, not the report. Five [SEO consultant services](https://scalewithsearch.com/seo), scoped per job:

- [Technical SEO](https://scalewithsearch.com/seo/technical-seo): Google, ChatGPT, or an AI crawler cannot reach, render, or index the pages.
- [On-page and content SEO](https://scalewithsearch.com/seo/on-page-and-content-seo): the pages say the wrong thing, say it late, or say it without a date or a source.
- [Semantic SEO and topical authority](https://scalewithsearch.com/seo/semantic-seo-and-topical-authority): the site covers its subject in pieces, so a competitor is the answer.
- [Custom SEO tools](https://scalewithsearch.com/seo/custom-seo-tools): the data exists, and no page or tool turns it into visits the business owns.
- [YouTube AI visibility](https://scalewithsearch.com/seo/youtube-ai-visibility): which videos AI answers cite, and who gets cited instead.

**One AI function.** For teams of 5 to 30 where leads come in faster than one person can route them. [AI operations](https://scalewithsearch.com/ai-systems), one recurring job at a time: lead routing, speed to lead, follow-up drafts, or lead reporting, run from files the business owns, with a person at both ends.

Neither job requires the other. Both start with a six-question brief. The scope comes back in writing with a fixed price, and nothing starts until it is accepted in writing.

## How I work

I scope the job, decide what changes, and review every output before it ships. AI agents I run in parallel do the volume: the crawls, the first drafts, the schema, the checks. There is no account manager and no retainer. The method is public, and the files stay with the client.

Four rules hold on every job:

- **One current record.** Every fact has one current version, in a file the business owns. The pages, the listings, and any AI pointed at the record read from the same place.
- **Fix the source before the symptom.** Rankings and AI answers follow what the engines can read. A report describes the problem. It does not fix it.
- **Approval at the action boundary.** Sends, publishing, purchases, deletions, and live account changes wait for a named person to approve them.
- **People at both ends.** A person gives the direction. A person checks the result before anything leaves the business.

## The tools

The method, in code. Each repository came out of my own work and fixes one problem that work hit.

| Repository | What it does | Where it fits |
| --- | --- | --- |
| [content-brief-dfs](https://github.com/b2bvic/content-brief-dfs) | Surfer- and Clearscope-style content briefs, computed from the DataForSEO API. Measures the ranking pages: term ranges, entities, topic coverage, and the searches ChatGPT runs for the keyword. Marks the questions no page answers, and scores a draft. About $0.05 a keyword. | On-page and content SEO |
| [seo-checks](https://github.com/b2bvic/seo-checks) | Twenty SEO page checks from one command: `seo-checks robots`, `seo-checks redirects`, `seo-checks schema-product`, and 17 more, each with JSON output. | Technical SEO |
| [owned-record](https://github.com/b2bvic/owned-record) | Keeps business context in Markdown and Claude Code and Codex transcripts in SQLite with full-text search. Change the model or the vendor; the record stays. | Own: the record |
| [agent-oversight](https://github.com/b2bvic/agent-oversight) | Checks agent work from outside the agent. Scores responses against writing rules, lists running Claude Code and Codex sessions, binds review receipts to file hashes, and holds REST writes in dry-run until a person enables them. | Approval at the action boundary |
| [vault-crawl](https://github.com/b2bvic/vault-crawl) | A Rust retrieval core: fetched pages stored with provenance, content-addressed blobs, and SQLite search. | Find: what the engines read |
| [declip](https://github.com/b2bvic/declip) | Plans filler, silence, and retake cuts in local audio or video with Whisper and ffmpeg. You accept or reject every cut on a local review page before it renders. | Video |
| [ops-scripts](https://github.com/b2bvic/ops-scripts) | Five operator scripts: Telegram alerts, Linux host checks, a macOS Messages export, an X bookmark import, and an X posting queue. Each README states what it reads and writes. | Operations |

The site sources for [polytraffic](https://github.com/b2bvic/polytraffic), [creatinepedia](https://github.com/b2bvic/creatinepedia), [ivibecodeditforyou](https://github.com/b2bvic/ivibecodeditforyou), and [AIPayPerCrawl](https://github.com/b2bvic/AIPayPerCrawl) hold the Markdown and build scripts for content sites on the same stack.

The 39 earlier single-tool repositories are archived. Each archived README names its new home: `observer-daemon` is now in `agent-oversight`, `sitemap-check` is `seo-checks sitemap`, and `session-ledger` is in `owned-record`.

## Provenance

This README was written with model assistance from the current repository files and the live pages of scalewithsearch.com. Each repository README is the authority on its setup, data boundaries, and limits. [EVIDENCE.md](EVIDENCE.md) links the source lines behind the tool claims on this page.
