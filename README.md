# Chameleon Cowork Marketplace

A plugin marketplace for [Claude Cowork](https://claude.com/claude-code) by **fenixstarlord** — post-production plugins for DaVinci Resolve and Frame.io.

## Plugins

### davinci-resolve

Control DaVinci Resolve from Cowork — execute API calls, create timelines, manage media, and render projects.

**Repo:** [fenixstarlord/cowork-davinciresolve](https://github.com/fenixstarlord/cowork-davinciresolve)

### frameio

Frame.io integration for Cowork — upload assets, manage reviews, collect feedback, and orchestrate approval workflows via the Frame.io V4 API.

**Repo:** [fenixstarlord/cowork-frameio](https://github.com/fenixstarlord/cowork-frameio)

## Marketplace Manifest

The marketplace is defined in `.claude-plugin/marketplace.json`. Cowork reads this file to discover available plugins and their source repositories.

## Adding a Plugin

Add an entry to the `plugins` array in `.claude-plugin/marketplace.json`:

```json
{
  "name": "your-plugin-name",
  "source": {
    "source": "github",
    "repo": "fenixstarlord/your-plugin-repo"
  },
  "description": "What the plugin does"
}
```

## License

MIT
