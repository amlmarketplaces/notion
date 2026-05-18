# amlmarketplaces/notion

Claude Code marketplace federating all `@amlplugins/notion-*` plugins.

## Install

Add to your project's `.claude/settings.json`:

```json
{
  "extraKnownMarketplaces": {
    "aml-notion": {
      "source": { "source": "github", "repo": "amlmarketplaces/notion" }
    }
  },
  "enabledPlugins": {
      "notion-blocks@aml-notion": true,
      "notion-comments@aml-notion": true,
      "notion-databases@aml-notion": true,
      "notion-pages@aml-notion": true,
      "notion-search@aml-notion": true
    }
}
```

Then launch Claude Code in the project. The marketplace is fetched from `amlmarketplaces/notion`, cached under `~/.claude/plugins/cache/aml-notion/`, and each enabled plugin is loaded from its `amlplugins` source repo.

## Plugins (6 total)

- `notion-blocks` — [@amlplugins/notion-blocks](https://github.com/amlplugins/notion-blocks)
- `notion-comments` — [@amlplugins/notion-comments](https://github.com/amlplugins/notion-comments)
- `notion-databases` — [@amlplugins/notion-databases](https://github.com/amlplugins/notion-databases)
- `notion-pages` — [@amlplugins/notion-pages](https://github.com/amlplugins/notion-pages)
- `notion-search` — [@amlplugins/notion-search](https://github.com/amlplugins/notion-search)
- `notion-users` — [@amlplugins/notion-users](https://github.com/amlplugins/notion-users)

## Related

- npm packages: `@amlplugins/notion-*` published to GitHub Packages (`https://npm.pkg.github.com`).
- Aggregating parent: [`amlmarketplaces/aml`](https://github.com/amlmarketplaces/aml) — federates every `@amlplugins/*` plugin under a single marketplace.
- AML topology: see `.claude/rules/definitions/ageni.md` § "GitHub Topology" — this repository is a Tier-4 HUB-INSTANCE under the `amlmarketplaces/` Tier-3 HUB-ORGANIZATION.

> Built by `.claude/skills/aml/metateam/marketplace/test/cross-org-amlmarketplaces-batch.mjs`.
