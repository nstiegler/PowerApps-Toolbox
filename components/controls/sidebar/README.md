# Sidebar

Collapsible navigation sidebar with icon and label menu items.

## Preview

A dark vertical sidebar that expands/collapses via hamburger icon. Contains two menu sections ("Main" and "Workspace") with icon+label navigation items. Shows current user's name at bottom when expanded.

## Tags

`ui` `navigation` `layout`

## Required Variables

| Variable | Type | Purpose |
|----------|------|---------|
| `varSidebar` | Boolean | Controls expanded (true) vs collapsed (false) state |

## Setup

1. Add to `App.OnStart` or `Screen.OnVisible`:
   ```
   UpdateContext({ varSidebar: true })
   ```

2. Copy contents of `sidebar.yaml` and paste into your screen

3. Customize menu items:
   - Update `Text` on label controls (`lblItem2`, `lblItem3`, etc.)
   - Change `Icon` property on icon controls
   - Add `OnSelect` logic to `Button1`, `Button2`, etc.

4. Update title: Change `Text` on `lblTitle` (default: "App Name")

## Customization

- **Width:** Modify the `Width` formula on `conSidebar` (default: 17% expanded, 5% collapsed)
- **Colors:** Change `Fill` on `conSidebar` (default: dark gray #1A1A1A)
- **Add sections:** Duplicate `conBlock1` or `conBlock2` containers
- **Add menu items:** Duplicate `conBlock1ItemCon` pattern
- **Icons:** Use Power Apps `Icon` enum values

## Menu Structure

```
conSidebar
├── conTitle (logo + title + hamburger)
├── conItems
│   ├── conBlock1 ("Main" section)
│   │   ├── Home
│   │   ├── Dashboard
│   │   └── Analytics
│   ├── conBlock2 ("Workspace" section)
│   │   ├── Teams
│   │   ├── Messages
│   │   └── Settings
│   └── conSpacing (flexible spacer)
└── conUser (current user name)
```

## Dependencies

- Uses `User().FullName` for displaying current user
