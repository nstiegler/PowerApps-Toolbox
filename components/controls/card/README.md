# Card

Container card with form fields and action buttons.

## Preview

A white card with drop shadow containing a title, subtitle, two labeled text inputs, and Cancel/Deploy buttons.

## Tags

`ui` `layout` `container` `form`

## Required Variables

None

## Setup

1. Copy contents of `card.yaml` and paste into your screen

2. Customize labels and placeholder text:
   - `lblTitle` — Card heading
   - `lblTitle2` — Subtitle/description
   - `lblItem1`, `lblItem2` — Field labels
   - `txtItem1.HintText`, `txtItem2.HintText` — Placeholder text

3. Add your logic to `btnDeploy.OnSelect` and `btnCancel.OnSelect`

## Customization

- **Size:** Adjust `Width` and `Height` on `conCard`
- **Shadow:** Change `DropShadow` property (None, Light, Regular, Bold)
- **Corners:** Modify radius properties (default: 15)
- **Add fields:** Duplicate `txtItem` and `lblItem` pairs, adjust Y positions

## Dependencies

None
