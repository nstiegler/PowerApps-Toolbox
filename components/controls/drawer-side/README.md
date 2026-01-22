# Drawer Side

Side panel drawer with backdrop overlay.

## Preview

A panel that slides in from the right side of the screen with a semi-transparent backdrop. Contains sample form fields and action buttons. Includes trigger button.

## Tags

`ui` `overlay` `navigation`

## Required Variables

| Variable | Type | Purpose |
|----------|------|---------|
| `showDrawer` | Boolean | Controls drawer visibility |

## Setup

1. Add to `App.OnStart` or `Screen.OnVisible`:
   ```
   UpdateContext({ showDrawer: false })
   ```

2. Copy contents of `drawer-side.yaml` and paste into your screen

3. Customize drawer content (labels, inputs, buttons)

4. Optionally remove `btnDrawer` trigger button and use your own trigger

## Customization

- **Width:** Adjust `Width` on `conDrawer` (default: 324)
- **Position:** Modify `X` on `conDrawer` to change horizontal position
- **Corners:** Modify `RadiusTopLeft` and `RadiusBottomLeft` (default: 20)
- **Backdrop:** Change `Fill` opacity on `recBackground` (default: 0.2)
- **Side:** To slide from left, set `X: 0` and change radius to right corners

## Components

- `recBackground` — Backdrop overlay
- `conDrawer` — Main drawer container with form
- `btnDeploy` / `btnCancel` — Action buttons (close drawer)
- `btnDrawer` — Sample trigger button (can be removed)

## Dependencies

None
