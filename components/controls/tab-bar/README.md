# Tab Bar

Horizontal tab navigation.

## Preview

A gray container with two tab buttons. Selected tab has white background; unselected tabs are gray. Useful for switching between content views.

## Tags

`ui` `navigation`

## Required Variables

| Variable | Type | Purpose |
|----------|------|---------|
| `selectedTab` | Number | Tracks active tab (1 or 2) |

## Setup

1. Add to `App.OnStart` or `Screen.OnVisible`:
   ```
   UpdateContext({ selectedTab: 1 })
   ```

2. Copy contents of `tab-bar.yaml` and paste into your screen

3. Update tab labels: Change `Text` on `btn1` and `btn2`

4. Use `selectedTab` to control content visibility:
   ```
   // On your content containers:
   Visible: selectedTab = 1
   Visible: selectedTab = 2
   ```

## Customization

- **Add tabs:** Duplicate `btn2`, update `OnSelect` to set `selectedTab: 3`, etc.
- **Colors:** Modify `Fill` formulas for selected/unselected states
- **Width:** Adjust `Width` on `conTab` container
- **Styling:** Change `RadiusBottomLeft`, etc. for different corner styles

## Dependencies

None
