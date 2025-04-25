# Contributing to PowerApps-Toolbox

Thank you for your interest in contributing to the PowerApps-Toolbox! This repository is a collection of reusable Power Apps components, solutions, flows, scripts, and templates. We welcome contributions that add value, improve existing assets, or share new reusable resources.

## Table of Contents
- [How to Contribute](#how-to-contribute)
- [Contribution Guidelines](#contribution-guidelines)
- [Submitting a Contribution](#submitting-a-contribution)
- [Code of Conduct](#code-of-conduct)
- [Questions?](#questions)

## How to Contribute
You can contribute by:
- Adding new reusable assets (e.g., canvas apps, flows, connectors, scripts, or templates).
- Improving existing assets (e.g., bug fixes, performance enhancements).
- Updating documentation (e.g., `CATALOG.md`, asset READMEs, or guides).
- Suggesting new ideas via GitHub Issues.

## Contribution Guidelines
To ensure consistency and quality, please follow these guidelines:
1. **Asset Requirements**:
   - Assets should be reusable, modular, and well-documented.
   - Include a `README.md` in the asset’s folder with:
     - Purpose of the asset.
     - Setup instructions.
     - Dependencies (e.g., connectors, environment settings).
     - Example use case.
   - Use descriptive names (e.g., `Employee_Onboarding_Flow.zip`).
   - Tag assets in [CATALOG.md](./CATALOG.md) with relevant tags (e.g., `#HR #Flow`).

2. **File Organization**:
   - Place assets in the appropriate folder:
     - `/components`: Canvas apps, flows, connectors, controls.
     - `/solutions`: Domain-specific solutions (e.g., `/hr`, `/finance`).
     - `/scripts`: Automation scripts.
     - `/templates`: Boilerplate files.
   - Update [CATALOG.md](./CATALOG.md) with the new asset’s details.

3. **Documentation**:
   - Keep documentation clear and concise.
   - Update `/docs/guides` if your contribution introduces new processes or tools.

4. **Best Practices**:
   - Avoid hardcoding environment-specific details (e.g., URLs, API keys).
   - Test assets before submitting to ensure they import and function correctly.
   - Use Power Platform CLI for exporting solutions or flows where applicable.

5. **Version Control**:
   - Use semantic versioning (e.g., v1.0.0) for updated assets.
   - Commit exported solution files (.zip) or unpacked files for tracking changes.

## Submitting a Contribution
1. **Fork the Repository**:
   - Fork the `PowerApps-Toolbox` repository to your GitHub account.

2. **Create a Branch**:
   - Create a descriptive branch name (e.g., `add-onboarding-flow`).
   - Example: `git checkout -b add-onboarding-flow`

3. **Add Your Contribution**:
   - Place your asset in the correct folder.
   - Update [CATALOG.md](./CATALOG.md) and include a `README.md` for the asset.
   - Test your changes locally (e.g., import the asset to verify it works).

4. **Commit Changes**:
   - Write clear commit messages (e.g., `Add Employee Onboarding Flow with SharePoint integration`).
   - Example: `git commit -m "Add Employee Onboarding Flow with SharePoint integration"`

5. **Push and Create a Pull Request**:
   - Push your branch: `git push origin add-onboarding-flow`
   - Open a pull request (PR) on GitHub with:
     - A description of the contribution.
     - Reference to any related issues (e.g., `Fixes #123`).
     - Screenshots or examples (if applicable).

6. **Review Process**:
   - Maintainers will review your PR and may request changes.
   - Once approved, your contribution will be merged into the main branch.

## Code of Conduct
- Be respectful and inclusive in all interactions.
- Follow GitHub’s [Community Guidelines](https://docs.github.com/en/site-policy/github-terms/github-community-guidelines).
- Report any issues to the repository maintainers via GitHub Issues.

## Questions?
If you have questions or need help, please:
- Open an issue with the `question` label.
- Reach out via [LinkedIn/X/Power Apps Community] (replace with preferred contact method).

Thank you for helping make PowerApps-Toolbox a valuable resource for the Power Apps community!
