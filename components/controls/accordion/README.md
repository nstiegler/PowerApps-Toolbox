# Accordion

Expandable/collapsible content sections with animated chevron icons.

## Preview

A vertical stack of 3 collapsible panels. Clicking a header expands that section and collapses others. Chevron icon animates on toggle.

## Tags

`ui` `layout` `expandable`

## Required Variables

| Variable | Type | Purpose |
|----------|------|---------|
| `openAccordion` | Number | Tracks which section is open (1, 2, 3, or Blank) |
| `arrowTimestamp1` | Text | Animation trigger for section 1 |
| `arrowTimestamp2` | Text | Animation trigger for section 2 |
| `arrowTimestamp3` | Text | Animation trigger for section 3 |

## Setup

1. Add to `App.OnStart` or `Screen.OnVisible`:
   ```
   UpdateContext({
       openAccordion: Blank(),
       arrowTimestamp1: Blank(),
       arrowTimestamp2: Blank(),
       arrowTimestamp3: Blank()
   })
   ```

2. Copy contents of `accordion.yaml` and paste into your screen

3. Customize header text (`lblHeader1`, `lblHeader2`, `lblHeader3`) and body text (`lblBody1`, `lblBody2`, `lblBody3`)

## Customization

- **Add/remove sections:** Duplicate or delete `con1`/`con2`/`con3` containers. Update variable references accordingly.
- **Change colors:** Modify `Fill` and `BorderColor` properties on `recDivider` elements
- **Adjust sizing:** Modify `Height` values in container properties (default: 60px collapsed, 100px expanded)

## Dependencies

None
