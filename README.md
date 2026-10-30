# my-mods

Two Claude Code mods, edited copies of others' work (both MIT, licenses kept in each folder):

- **ribbon**: usage band above the prompt (5H / 7D % used, prompt-cache warm or cold). From [robonuggets/ribbon](https://github.com/robonuggets/ribbon).
- **savvy-progress**: progress bar and agents panel for subagents. From [johnnyvizz/claude-kit](https://github.com/johnnyvizz/claude-kit/tree/main/plugins/savvy-progress).

## Install

At the prompt of a terminal session:

```
/plugin install ribbon --marketplace HUNGRYARMY/claude-mods
/plugin install savvy-progress --marketplace HUNGRYARMY/claude-mods
```

From a shell:

```
claude plugin install ribbon --marketplace HUNGRYARMY/claude-mods
claude plugin install savvy-progress --marketplace HUNGRYARMY/claude-mods
```

In the desktop app: click + next to the prompt box, then Plugins, Add marketplace with `HUNGRYARMY/claude-mods`, then Add plugin.

For cloud sessions, add this to a repository's `.claude/settings.json`:

```json
{
  "extraKnownMarketplaces": {
    "my-mods": { "source": { "source": "github", "repo": "HUNGRYARMY/claude-mods" } }
  },
  "enabledPlugins": { "ribbon@my-mods": true, "savvy-progress@my-mods": true }
}
```
