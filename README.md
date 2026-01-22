# PowerApps-Toolbox

A curated collection of reusable Power Apps components, solutions, flows, scripts, and templates for rapid development and reference.

## Table of Contents
- [Overview](#overview)
- [Getting Started](#getting-started)
- [Repository Structure](#repository-structure)
- [How to Use Assets](#how-to-use-assets)
- [Contributing](#contributing)
- [License](#license)
- [Contact](#contact)

## Overview

This repository serves as a personal toolbox for Power Apps developers, containing reusable canvas apps, Power Automate flows, custom connectors, solutions, scripts, and templates. Whether you're building HR solutions, finance workflows, or general-purpose apps, these assets are designed to save time and provide reliable starting points.

## Getting Started

1. **Prerequisites**:
   - Power Apps account with access to your environment.
   - [Power Platform CLI](https://learn.microsoft.com/en-us/power-platform/developer/cli/introduction) installed for importing/exporting assets.
   - Basic knowledge of Power Apps, Power Automate, and Git.

2. **Clone the Repository**:
   ```bash
   git clone https://github.com/nstiegler/PowerApps-Toolbox.git
   ```

3. **Explore Assets**:
   - Browse the [Asset Catalog](./docs/CATALOG.md) to find components, solutions, or scripts.
   - Check `/docs/guides` for detailed setup and customization instructions.

## Repository Structure

```
PowerApps-Toolbox/
├── components/
│   ├── controls/      ← YAML snippets for Canvas Apps
│   └── flows/         ← (coming soon)
├── solutions/         ← (coming soon)
├── scripts/           ← (coming soon)
├── templates/         ← (coming soon)
└── docs/
    ├── CATALOG.md     ← Index of all assets
    └── guides/        ← How-to guides
```

| Folder | Purpose |
|--------|---------|
| `/components` | Reusable canvas apps, flows, connectors, and controls |
| `/solutions` | Domain-specific solutions (e.g., HR, finance) |
| `/scripts` | Automation scripts for exporting, deploying, or configuring assets |
| `/templates` | Boilerplate files for starting new projects |
| `/docs` | Documentation, including guides and the asset catalog |

## How to Use Assets

1. **Find an Asset**:
   - Use the [Asset Catalog](./docs/CATALOG.md) to locate components or solutions by name, tag, or category.

2. **Import an Asset**:
   - For solutions: `pac solution import --path ./solutions/hr/HR_Onboarding.zip`
   - For flows: Import `.zip` files via Power Automate.
   - For canvas apps: Import `.msapp` files via Power Apps.
   - For controls: Copy YAML from the control's folder and paste into Power Apps Studio (Tree View).

3. **Customize**:
   - Follow the `README.md` in each asset's folder for setup and customization instructions.

## Contributing

Want to add your own reusable assets? See [CONTRIBUTING.md](./CONTRIBUTING.md) for guidelines on submitting components, solutions, or scripts.

## License

This project is licensed under the [MIT License](./LICENSE.md).

## Contact

Questions or suggestions? Open an issue on GitHub.
