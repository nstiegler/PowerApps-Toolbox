# Controls

Reusable Canvas App UI controls in YAML format.

## Usage

1. Open your Canvas App in Power Apps Studio
2. Switch to the Tree View
3. Select a screen or container
4. Paste the YAML content from the control's `.yaml` file

## Available Controls

| Control | Description | Variables Required |
|---------|-------------|-------------------|
| [accordion](./accordion/) | Expandable/collapsible sections | Yes |
| [button](./button/) | Basic filled button | No |
| [button-dropdowns](./button-dropdowns/) | Button with dropdown menu | Yes |
| [button-outline](./button-outline/) | Outlined/ghost button | No |
| [card](./card/) | Container card with form | No |
| [drawer-bottom](./drawer-bottom/) | Bottom sheet drawer | Yes |
| [drawer-side](./drawer-side/) | Side panel drawer | Yes |
| [input](./input/) | Text input field | No |
| [modal](./modal/) | Popup dialog | Yes |
| [sidebar](./sidebar/) | Collapsible nav sidebar | Yes |
| [tab-bar](./tab-bar/) | Tab navigation | Yes |
| [toast](./toast/) | Notification toast | Yes |
| [toggle](./toggle/) | On/off toggle button | Yes |

Each control folder contains:
- `README.md` — Purpose, setup, required variables, customization tips
- `*.yaml` — The control code to copy/paste
