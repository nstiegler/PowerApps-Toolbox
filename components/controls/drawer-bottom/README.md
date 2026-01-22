# Drawer Bottom

Bottom sheet drawer with backdrop overlay.

## Preview

A panel that slides up from the bottom of the screen with a semi-transparent backdrop. Contains sample form fields. Includes trigger button.

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

2. Copy contents of `drawer-bottom.yaml` and paste into your screen

3. Customize drawer content (labels, inputs, buttons)

4. Optionally remove `btnDrawer` trigger button and use your own trigger

## Customization

- **Height:** Adjust `Height` on `conDrawer` (default: 316)
- **Corners:** Modify `RadiusTopLeft` and `RadiusTopRight` (default: 20)
- **Backdrop:** Change `Fill` opacity on `recBackground` (default: 0.2)
- **Position:** Adjust `Y` on `conDrawer` to control vertical position

## Components

- `recBackground` — Backdrop overlay (click to close optional)
- `conDrawer` — Main drawer container
- `btnDrawer` — Sample trigger button (can be removed)

## Dependencies

None
