# Contributing to PowerApps-Toolbox

Guidelines for adding assets to this repository.

## Adding a New Control

1. Create a folder in `/components/controls/` with kebab-case name (e.g., `my-control/`)

2. Add your files:
   - `my-control.yaml` — The control code
   - `README.md` — Documentation (use existing controls as template)

3. Update `/components/controls/README.md` table

4. Add entry to `/docs/CATALOG.md`:
   - Quick reference table row
   - Detailed section with tags, variables, setup

## README Template for Controls

```markdown
# Control Name

Brief description of what it does.

## Preview

What it looks like / how it behaves.

## Tags

`tag1` `tag2` `tag3`

## Required Variables

| Variable | Type | Purpose |
|----------|------|---------|
| `varName` | Type | What it controls |

## Setup

1. Add to `App.OnStart` or `Screen.OnVisible`:
   \`\`\`
   UpdateContext({ varName: initialValue })
   \`\`\`

2. Copy contents of `control-name.yaml` and paste into your screen

3. Customize...

## Customization

- **Property:** How to change it

## Dependencies

None (or list any)
```

## Naming Conventions

- Folders and files: `kebab-case` (lowercase, hyphens)
- Tags: lowercase, single words
- Variables: `camelCase`

## Best Practices

- Avoid hardcoding environment-specific values (URLs, keys)
- Document all required context variables
- Test that YAML imports cleanly before committing
