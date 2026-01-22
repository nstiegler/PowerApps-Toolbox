# PowerApps-Toolbox

A personal library of reusable Power Platform snippets and components—designed for quick copy-paste during development.

## Quick Start

1. Browse the [Asset Catalog](./docs/CATALOG.md) to find what you need
2. Open the `.yaml` file for any control
3. Copy and paste directly into Power Apps Studio (Tree View)

## What's Here

**Currently available:**
- `/components/controls/` — 13 Canvas App UI controls (buttons, modals, drawers, sidebar, etc.)

**Scaffolded for future use:**
- `/components/flows/` — Power Automate flows
- `/solutions/` — Domain-specific solution packages
- `/scripts/` — Automation and deployment scripts
- `/templates/` — Boilerplate starters

## Repository Structure

```
PowerApps-Toolbox/
├── components/
│   ├── controls/      ← YAML snippets for Canvas Apps
│   └── flows/         ← (coming soon)
├── solutions/         ← (coming soon)
├── scripts/           ← (coming soon)
├── templates/         ← (coming soon)
└── docs/
    ├── CATALOG.md     ← Index of all assets
    └── guides/        ← How-to guides
```

## Using Controls

1. Open your Canvas App in Power Apps Studio
2. Switch to **Tree View**
3. Select a screen or container
4. Paste the YAML content

Most controls require context variables (e.g., `showModal`, `selectedTab`). Check each control's entry in the [Catalog](./docs/CATALOG.md) for required variables.

## Contributing

See [CONTRIBUTING.md](./CONTRIBUTING.md) for guidelines. The short version: add your asset to the right folder, document it, and update the catalog.

## License

[MIT License](./LICENSE.md)
