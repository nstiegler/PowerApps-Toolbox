# Button Dropdowns

Menu bar with dropdown menus (File/Edit style).

## Preview

Two buttons ("File", "Edit") that reveal dropdown menus when clicked. Menus contain sample actions like New Tab, Undo, Copy, etc.

## Tags

`ui` `navigation` `menu`

## Required Variables

| Variable | Type | Purpose |
|----------|------|---------|
| `showDropdown` | Boolean | Controls "Edit" dropdown visibility |
| `showDropdown1` | Boolean | Controls "File" dropdown visibility |

## Setup

1. Add to `App.OnStart` or `Screen.OnVisible`:
   ```
   UpdateContext({
       showDropdown: false,
       showDropdown1: false
   })
   ```

2. Copy contents of `button-dropdowns.yaml` and paste into your screen

3. Customize menu items by updating `Text` properties on `btnItem` buttons

4. Add your logic to each menu item's `OnSelect`

## Customization

- **Add menu items:** Duplicate `btnItem` controls within dropdown containers
- **Change menu labels:** Update `Text` on `btn1` and `btn2`
- **Styling:** Modify `Fill`, `HoverFill` on dropdown containers and items
- **Width:** Adjust `Width` on `conDropdown` and `conDropdown1`

## Dependencies

None
