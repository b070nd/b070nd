# Botond Biro

I build local-first tools in Go for people who have to answer for what ships:
what changed, who approved it, what is still exposed, and what a model actually
said. Twenty years of backend engineering; these tools are what I built for the
problems I ran into.

[![LinkedIn](https://img.shields.io/badge/LinkedIn-botondbiro-0A66C2?logo=linkedin&logoColor=white)](https://www.linkedin.com/in/botondbiro/)
[![XERJ Corpus Hub contributor](https://hub.xerj.org/contributors/b070nd/badge.svg)](https://hub.xerj.org/contributors/b070nd)

## stAirCase

**AI agents propose. You approve. Only what you approved is committed, and you can prove it.**

[![CI](https://github.com/b070nd/stAirCase/actions/workflows/ci.yml/badge.svg)](https://github.com/b070nd/stAirCase/actions/workflows/ci.yml)
[![CodeQL](https://github.com/b070nd/stAirCase/actions/workflows/codeql.yml/badge.svg)](https://github.com/b070nd/stAirCase/actions/workflows/codeql.yml)
[![OpenSSF Scorecard](https://api.securityscorecards.dev/projects/github.com/b070nd/stAirCase/badge)](https://scorecard.dev/viewer/?uri=github.com/b070nd/stAirCase)
[![Release](https://img.shields.io/github/v/release/b070nd/stAirCase)](https://github.com/b070nd/stAirCase/releases/latest)

[stAirCase](https://github.com/b070nd/stAirCase) sits between an AI coding agent
and your git repository. The agent works in a separate copy, every change waits
for a decision, and the final commit carries a signed change certificate that
anyone can verify and rebuild.

```bash
brew install b070nd/staircase/staircase
staircase claude "add a /health endpoint that returns 200"
staircase verify staircase/run-1
```

Releases for macOS, Linux and Windows, with Sigstore-signed checksums and an SBOM
for every archive. More than 1,100 tests. I use it on my own projects.

- [stAirCase-skills](https://github.com/b070nd/stAirCase-skills): Claude Code skills for the stAirCase workflows
- [Quickstart](https://github.com/b070nd/stAirCase/blob/main/QUICKSTART.md) · [Roadmap](https://github.com/b070nd/stAirCase/blob/main/ROADMAP.md)

## Other projects

| Project | What it does | State |
|---|---|---|
| [cvewatch](https://github.com/b070nd/cvewatch) | Tracks which of your projects and environments are still exposed to which CVE, and who owns the fix. Terminal UI and MCP tools. | v2.1.0, six platforms, 1,200+ tests. Selected for the [XERJ Corpus Hub](https://hub.xerj.org/contributors/b070nd) |
| [stoxicity](https://github.com/b070nd/stoxicity) | News and portfolio research for long-term stock investors, from primary sources, in a local terminal app. | Working, tested in CI; no release yet |
| [motiv-cell](https://github.com/b070nd/motiv-cell) | Experiment: deterministic cells for actors and motivations in text. Model answers are recorded and replay byte for byte. | Working pipeline at small scale; no evaluation yet |

## How I work

I build with AI coding agents and keep the engineering decisions: I write the
specifications and design records, review every diff, and nothing is released
until the full test suite passes. stAirCase exists because I needed that gate
for myself.

## Get in touch

Issues and discussions on the repos are the best way to reach me about the
projects. For anything else, [LinkedIn](https://www.linkedin.com/in/botondbiro/).
