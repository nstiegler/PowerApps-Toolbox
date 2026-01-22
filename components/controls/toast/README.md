# Toast

Notification toast message.

## Preview

A small card positioned at bottom-right with title, body text, and an action button. Appears/disappears based on state. Includes trigger button.

## Tags

`ui` `notification` `feedback`

## Required Variables

| Variable | Type | Purpose |
|----------|------|---------|
| `showToast` | Boolean | Controls toast visibility |

## Setup

1. Add to `App.OnStart` or `Screen.OnVisible`:
   ```
   UpdateContext({ showToast: false })
   ```

2. Copy contents of `toast.yaml` and paste into your screen

3. Customize content:
   - `lblTitle` — Notification heading
   - `lblBody` — Notification message
   - `btnUndo` — Action button (text and OnSelect)

4. Trigger the toast from your app logic:
   ```
   UpdateContext({ showToast: true })
   ```

5. Optionally remove `btnToast` sample trigger

## Customization

- **Position:** Adjust `X` and `Y` on `conToast` (default: bottom-right)
- **Size:** Modify `Width` and `Height` on `conToast`
- **Auto-dismiss:** Add a Timer control that sets `showToast: false` after delay
- **Colors:** Change `Fill` on `conToast` and button colors

## Auto-Dismiss Pattern

To auto-hide after 3 seconds:
1. Add a Timer control
2. Set `Duration: 3000`
3. Set `Start: showToast`
4. Set `OnTimerEnd: UpdateContext({ showToast: false })`
5. Set `Reset: !showToast`

## Dependencies

None
