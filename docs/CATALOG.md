# Asset Catalog

A searchable index of all assets in this repository.

## Quick Reference

| Asset | Type | Tags | Variables Required |
|-------|------|------|-------------------|
| [accordion](#accordion) | Control | `ui` `layout` `expandable` | `openAccordion`, `arrowTimestamp1`, `arrowTimestamp2`, `arrowTimestamp3` |
| [button](#button) | Control | `ui` `input` `basic` | None |
| [button-dropdowns](#button-dropdowns) | Control | `ui` `navigation` `menu` | `showDropdown`, `showDropdown1` |
| [button-outline](#button-outline) | Control | `ui` `input` `basic` | None |
| [card](#card) | Control | `ui` `layout` `container` `form` | None |
| [drawer-bottom](#drawer-bottom) | Control | `ui` `overlay` `navigation` | `showDrawer` |
| [drawer-side](#drawer-side) | Control | `ui` `overlay` `navigation` | `showDrawer` |
| [input](#input) | Control | `ui` `form` `input` `basic` | None |
| [modal](#modal) | Control | `ui` `overlay` `dialog` | `showModal` |
| [sidebar](#sidebar) | Control | `ui` `navigation` `layout` | `varSidebar` |
| [tab-bar](#tab-bar) | Control | `ui` `navigation` | `selectedTab` |
| [toast](#toast) | Control | `ui` `notification` `feedback` | `showToast` |
| [toggle](#toggle) | Control | `ui` `input` `form` | `toggle` |

---

## Tags Index

### By Category
- **basic** — Simple, standalone controls: [button](#button), [button-outline](#button-outline), [input](#input)
- **container** — Wrapper/grouping controls: [card](#card)
- **dialog** — Modal dialogs: [modal](#modal)
- **expandable** — Expand/collapse behavior: [accordion](#accordion)
- **feedback** — User feedback elements: [toast](#toast)
- **form** — Form-related controls: [card](#card), [input](#input), [toggle](#toggle)
- **input** — User input controls: [button](#button), [button-outline](#button-outline), [input](#input), [toggle](#toggle)
- **layout** — Page structure controls: [accordion](#accordion), [card](#card), [drawer-bottom](#drawer-bottom), [drawer-side](#drawer-side), [sidebar](#sidebar)
- **menu** — Menu/dropdown patterns: [button-dropdowns](#button-dropdowns)
- **navigation** — Navigation elements: [button-dropdowns](#button-dropdowns), [drawer-bottom](#drawer-bottom), [drawer-side](#drawer-side), [sidebar](#sidebar), [tab-bar](#tab-bar)
- **notification** — Alerts and toasts: [toast](#toast)
- **overlay** — Overlays and modals: [drawer-bottom](#drawer-bottom), [drawer-side](#drawer-side), [modal](#modal)
- **ui** — All UI controls (all items)

---

## Controls

### accordion
**Path:** `components/controls/accordion/accordion.yaml`  
**Tags:** `ui` `layout` `expandable`

Expandable/collapsible content sections with animated chevron icons. Contains 3 accordion items by default.

**Required Variables:**
| Variable | Type | Purpose |
|----------|------|---------|
| `openAccordion` | Number | Tracks which section is open (1, 2, 3, or Blank) |
| `arrowTimestamp1` | Text | Animation trigger for section 1 |
| `arrowTimestamp2` | Text | Animation trigger for section 2 |
| `arrowTimestamp3` | Text | Animation trigger for section 3 |

**Setup:**
```
// Add to App.OnStart or Screen.OnVisible
UpdateContext({
    openAccordion: Blank(),
    arrowTimestamp1: Blank(),
    arrowTimestamp2: Blank(),
    arrowTimestamp3: Blank()
})
```

---

### button
**Path:** `components/controls/button/button.yaml`  
**Tags:** `ui` `input` `basic`

Basic filled button with rounded corners. Black fill, white text.

**Required Variables:** None

---

### button-dropdowns
**Path:** `components/controls/button-dropdowns/button-dropdowns.yaml`  
**Tags:** `ui` `navigation` `menu`

Two-button menu bar with dropdown menus (File, Edit style). Includes sample menu items.

**Required Variables:**
| Variable | Type | Purpose |
|----------|------|---------|
| `showDropdown` | Boolean | Controls "Edit" dropdown visibility |
| `showDropdown1` | Boolean | Controls "File" dropdown visibility |

**Setup:**
```
// Add to App.OnStart or Screen.OnVisible
UpdateContext({
    showDropdown: false,
    showDropdown1: false
})
```

---

### button-outline
**Path:** `components/controls/button-outline/button-outline.yaml`  
**Tags:** `ui` `input` `basic`

Ghost/outline button variant with transparent fill and visible border.

**Required Variables:** None

---

### card
**Path:** `components/controls/card/card.yaml`  
**Tags:** `ui` `layout` `container` `form`

Container card with drop shadow, title, subtitle, two form fields, and action buttons (Cancel/Deploy).

**Required Variables:** None

---

### drawer-bottom
**Path:** `components/controls/drawer-bottom/drawer-bottom.yaml`  
**Tags:** `ui` `overlay` `navigation`

Bottom sheet drawer with backdrop overlay. Slides up from bottom. Includes sample form content and trigger button.

**Required Variables:**
| Variable | Type | Purpose |
|----------|------|---------|
| `showDrawer` | Boolean | Controls drawer visibility |

**Setup:**
```
// Add to App.OnStart or Screen.OnVisible
UpdateContext({ showDrawer: false })
```

---

### drawer-side
**Path:** `components/controls/drawer-side/drawer-side.yaml`  
**Tags:** `ui` `overlay` `navigation`

Side panel drawer with backdrop overlay. Slides in from right. Includes sample form content, action buttons, and trigger button.

**Required Variables:**
| Variable | Type | Purpose |
|----------|------|---------|
| `showDrawer` | Boolean | Controls drawer visibility |

**Setup:**
```
// Add to App.OnStart or Screen.OnVisible
UpdateContext({ showDrawer: false })
```

---

### input
**Path:** `components/controls/input/input.yaml`  
**Tags:** `ui` `form` `input` `basic`

Basic text input field with border, hint text, and focus states.

**Required Variables:** None

---

### modal
**Path:** `components/controls/modal/modal.yaml`  
**Tags:** `ui` `overlay` `dialog`

Popup dialog with backdrop overlay, title, body text, and close button. Includes trigger button.

**Required Variables:**
| Variable | Type | Purpose |
|----------|------|---------|
| `showModal` | Boolean | Controls modal visibility |

**Setup:**
```
// Add to App.OnStart or Screen.OnVisible
UpdateContext({ showModal: false })
```

---

### sidebar
**Path:** `components/controls/sidebar/sidebar.yaml`  
**Tags:** `ui` `navigation` `layout`

Collapsible navigation sidebar with icon+label menu items. Expands/collapses via hamburger icon. Dark theme. Displays current user name.

**Required Variables:**
| Variable | Type | Purpose |
|----------|------|---------|
| `varSidebar` | Boolean | Controls expanded (true) vs collapsed (false) state |

**Setup:**
```
// Add to App.OnStart or Screen.OnVisible
UpdateContext({ varSidebar: true })
```

---

### tab-bar
**Path:** `components/controls/tab-bar/tab-bar.yaml`  
**Tags:** `ui` `navigation`

Horizontal tab bar with 2 tabs. Selected tab has white background; unselected is gray.

**Required Variables:**
| Variable | Type | Purpose |
|----------|------|---------|
| `selectedTab` | Number | Tracks active tab (1 or 2) |

**Setup:**
```
// Add to App.OnStart or Screen.OnVisible
UpdateContext({ selectedTab: 1 })
```

---

### toast
**Path:** `components/controls/toast/toast.yaml`  
**Tags:** `ui` `notification` `feedback`

Notification toast positioned at bottom-right. Includes title, body, action button, and trigger button.

**Required Variables:**
| Variable | Type | Purpose |
|----------|------|---------|
| `showToast` | Boolean | Controls toast visibility |

**Setup:**
```
// Add to App.OnStart or Screen.OnVisible
UpdateContext({ showToast: false })
```

---

### toggle
**Path:** `components/controls/toggle/toggle.yaml`  
**Tags:** `ui` `input` `form`

On/off toggle button. Changes appearance and text based on state.

**Required Variables:**
| Variable | Type | Purpose |
|----------|------|---------|
| `toggle` | Boolean | Tracks on/off state |

**Setup:**
```
// Add to App.OnStart or Screen.OnVisible
UpdateContext({ toggle: false })
```

---

## Flows

*No flows yet. Check back later or [contribute one](../CONTRIBUTING.md).*

---

## Solutions

*No solutions yet. Check back later or [contribute one](../CONTRIBUTING.md).*

---

## Scripts

*No scripts yet. Check back later or [contribute one](../CONTRIBUTING.md).*

---

## Templates

*No templates yet. Check back later or [contribute one](../CONTRIBUTING.md).*
