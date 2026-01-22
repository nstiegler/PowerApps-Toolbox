# Toggle

On/off toggle button.

## Preview

A button that switches between "On" and "Off" states. Changes color and text based on current state.

## Tags

`ui` `input` `form`

## Required Variables

| Variable | Type | Purpose |
|----------|------|---------|
| `toggle` | Boolean | Tracks on/off state |

## Setup

1. Add to `App.OnStart` or `Screen.OnVisible`:
   ```
   UpdateContext({ toggle: false })
   ```

2. Copy contents of `toggle.yaml` and paste into your screen

3. Use `toggle` variable in your app logic to respond to state changes

## Customization

- **Labels:** Change the `Text` formula: `If(toggle, "On", "Off")` → `If(toggle, "Enabled", "Disabled")`
- **Colors:** Modify the `Fill` and `Color` formulas for on/off states
- **Size:** Adjust `Width` and `Height`
- **Default state:** Set initial value in `UpdateContext`

## Example Usage

```
// Show/hide content based on toggle
Visible: toggle

// Conditional formatting
Fill: If(toggle, Color.Green, Color.Gray)

// Save toggle state
Patch(Settings, {FeatureEnabled: toggle})
```

## Dependencies

None
