# soli

Open-source tools that give AI agents original sources and evidence anyone can check.

An agent's answer is only as good as what it was given to read, and only as trustworthy as your ability to check it. Both projects here work on that: they hand the agent the original text, say exactly where it came from, and tell you when it is no longer current.

## [Paracortex](https://github.com/solisolsoli/paracortex)

**Your own notes, word for word.** Local search that gives an AI agent the original passages from your Markdown notes or Obsidian vault, each with its file path, line range and SHA-256 hash. A note that changed after indexing is held back until it is re-indexed. Command line, MCP server and prompt hook; runs on your machine and needs no API key.

<p align="center">
  <a href="https://github.com/solisolsoli/paracortex">
    <picture>
      <source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/solisolsoli/paracortex/main/docs/img/overview-dark.svg">
      <img src="https://raw.githubusercontent.com/solisolsoli/paracortex/main/docs/img/overview-light.svg" width="820"
           alt="A question goes to Paracortex on your machine, which searches your notes, follows your links and re-checks every hash, then hands the AI agent the original passages with their file path, line range and hash.">
    </picture>
  </a>
</p>

[Read me](https://github.com/solisolsoli/paracortex#readme) · [How retrieval works](https://github.com/solisolsoli/paracortex/blob/main/docs/retrieval.md) · [The integrity model](https://github.com/solisolsoli/paracortex/blob/main/docs/integrity.md) · [Measurements and limits](https://github.com/solisolsoli/paracortex/blob/main/docs/validation.md)

## [TimelineXray](https://github.com/solisolsoli/timelinexray)

**What X's published ranking code actually says.** A reader for the open-source recommendation code in `xai-org/x-algorithm` that ties every claim to exact lines at a pinned commit. When the code changes, the findings built on it are marked stale instead of quietly staying "true". Command line and read-only MCP server. Independent and unofficial; not affiliated with or endorsed by X or xAI.

<p align="center">
  <a href="https://github.com/solisolsoli/timelinexray">
    <picture>
      <source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/solisolsoli/timelinexray/main/docs/img/overview-dark.svg">
      <img src="https://raw.githubusercontent.com/solisolsoli/timelinexray/main/docs/img/overview-light.svg" width="820"
           alt="Published code at a pinned commit becomes exact spans; a finding cites those spans and is reviewed; when a newer commit changes the cited lines, the finding is marked stale.">
    </picture>
  </a>
</p>

[Read me](https://github.com/solisolsoli/timelinexray#readme) · [The evidence model](https://github.com/solisolsoli/timelinexray/blob/main/docs/evidence-model.md) · [Staleness](https://github.com/solisolsoli/timelinexray/blob/main/docs/staleness.md) · [Limits](https://github.com/solisolsoli/timelinexray/blob/main/docs/limits.md)

## Status

Both projects are in alpha. Each one documents what has been tested, how it was measured and where the limits are; those pages are part of the product, so read them before relying on a result.
