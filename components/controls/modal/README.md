# Modal

Popup dialog with backdrop overlay.

## Preview

A centered white dialog box with title, body text, and close button. Semi-transparent backdrop dims the screen. Includes trigger button.

## Tags

`ui` `overlay` `dialog`

## Required Variables

| Variable | Type | Purpose |
|----------|------|---------|
| `showModal` | Boolean | Controls modal visibility |

## Setup

1. Add to `App.OnStart` or `Screen.OnVisible`:
   ```
   UpdateContext({ showModal: false })
   ```

2. Copy contents of `modal.yaml` and paste into your screen

3. Customize content:
   - `lblTitle` — Dialog heading
   - `lblBody` — Dialog message
   - `btnCloseModal` — Close button text and action

4. Optionally remove `btnModal` trigger and use your own

## Customization

- **Size:** Adjust `Width` and `Height` on `conModalItems` (defaults to auto)
- **Corners:** Modify radius properties (default: 10)
- **Backdrop:** Change `Fill` opacity on `recDarken` (default: 0.2)
- **Add buttons:** Duplicate `btnCloseModal` for confirm/cancel pattern
- **Close on backdrop click:** Add `OnSelect: UpdateContext({ showModal: false })` to `recDarken`

## Components

- `btnModal` — Sample trigger button (can be removed)
- `recDarken` — Backdrop overlay
- `conModalItems` — Modal container with content

## Dependencies

None
