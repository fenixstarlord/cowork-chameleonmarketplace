# Chameleon Cowork Marketplace

## What This Project Is

A Claude Cowork plugin marketplace listing. This repo contains a `marketplace.json` manifest that registers plugins published by **fenixstarlord** so that Cowork can discover and install them.

This is NOT a plugin itself — it contains no skills, commands, agents, or MCP servers. It is a registry pointing to plugin repos hosted elsewhere on GitHub.

## Repository Structure

```
.claude-plugin/
  marketplace.json   ← The marketplace manifest (the only meaningful file)
```

## Registered Plugins

| Plugin | Repo | Description |
|--------|------|-------------|
| davinci-resolve | `fenixstarlord/cowork-davinciresolve` | Control DaVinci Resolve from Cowork — execute API calls, create timelines, manage media, and render projects |
| frameio | `fenixstarlord/cowork-frameio` | Frame.io integration for Cowork — video review, collaboration, uploads, feedback workflows |

## How to Update

To add a new plugin, append an entry to the `plugins` array in `.claude-plugin/marketplace.json` with `name`, `source` (GitHub repo), and `description`.

To remove a plugin, delete its entry from the array.

## Rules

- Keep `marketplace.json` valid JSON at all times.
- Every plugin entry must have `name`, `source.source`, `source.repo`, and `description`.
- Plugin names should be kebab-case and unique within the marketplace.
