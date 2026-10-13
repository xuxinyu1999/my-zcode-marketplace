# My ZCode Plugin Marketplace

A personal ZCode plugin marketplace.

## Install in ZCode

1. Open **Settings → Plugin Management → Discover**
2. Click the **`+`** button
3. Paste this repository's GitHub URL
4. Install plugins from the marketplace listing

## Structure

```
.
├── marketplace.json          # Marketplace manifest
└── plugins/
    └── hello-plugin/         # Example plugin
        ├── .zcode-plugin/
        │   └── plugin.json   # Plugin manifest
        └── skills/
            └── hello/
                └── SKILL.md  # Skill definition
```

## Adding a new plugin

1. Copy `plugins/hello-plugin` to `plugins/<your-plugin-name>`
2. Update `plugins/<your-plugin-name>/.zcode-plugin/plugin.json` (the `name` field must match `^[a-z0-9][a-z0-9._-]{0,127}$`)
3. Add an entry to the `plugins` array in `marketplace.json`
