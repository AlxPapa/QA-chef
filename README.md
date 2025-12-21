# QA-chef  (Software + Tools Installation)
this is a small read.me repo guide that includes various installation guides and links for QA setups 

A practical, OS-friendly checklist of tools I use for QA work (manual testing, test automation, API testing, performance testing, mobile testing, reporting, and CI/CD).

This repository is designed to be:
- ✅ Simple to follow (step-by-step installs)
- ✅ Cross-platform (Windows / macOS / Linux)
- ✅ Easy to extend as new tools are added

---

## Contents

- [Quick Start](#quick-start)
- [Core Tools (Recommended)](#core-tools-recommended)
- [Manual QA](#manual-qa)
- [Test Automation](#test-automation)
- [API Testing](#api-testing)
- [Performance Testing](#performance-testing)
- [Mobile Testing](#mobile-testing)
- [Databases & Data Tools](#databases--data-tools)
- [CI/CD & DevOps](#cicd--devops)
- [Reporting & Test Management](#reporting--test-management)
- [Nice-to-Have Utilities](#nice-to-have-utilities)
- [Verification Checklist](#verification-checklist)
- [Docs](#docs)
- [License](#license)

---

## Quick Start

### 1) Install a package manager
- **Windows:** Chocolatey or Winget  
- **macOS:** Homebrew  
- **Linux:** apt / dnf / pacman

> Tip: Once you have a package manager, most tools become 1-command installs.

### 2) Install core tools first
Install these before anything else:
- Git
- VS Code
- A terminal shell (PowerShell / zsh / bash)
- One automation runtime (Node.js OR Python)

---

## Core Tools (Recommended)

### Git
- Purpose: version control, PR workflows, collaboration
- Install: Git for your OS

### VS Code
- Purpose: editing, debugging, extensions for QA stacks
- Extensions (suggested):
  - Playwright Test for VS Code
  - Python
  - Pylance
  - ESLint
  - Prettier
  - GitLens
  - REST Client (optional)

### Runtimes
Choose what matches your automation stack:
- **Node.js (LTS)** + npm
- **Python 3.11+** + pip

### Browsers
- Google Chrome
- Microsoft Edge
- Mozilla Firefox

---

## Manual QA

### Tools
- **Snipping Tool / ShareX (Windows)** or native screenshot tools
- **OBS Studio (optional)** for recording repro steps
- **Postman / Insomnia** (also in API section)

### Documentation
- Markdown (README style notes)
- Optional: Notion / Confluence (team dependent)

---

## Test Automation

### Option A: Playwright (recommended modern E2E)
- Use-case: fast, reliable UI automation, cross-browser, great CI support
- Requirements:
  - Node.js (LTS)
  - Playwright

### Option B: Selenium
- Use-case: legacy projects, broad ecosystem, grid support
- Requirements:
  - Browser drivers (ChromeDriver / GeckoDriver) or Selenium Manager
  - Java or Python (depending on framework)

### Option C: Cypress (frontend-heavy web apps)
- Use-case: component/E2E testing for JS-first teams

---

## API Testing

### Postman
- Use-case: manual API testing, collections, environments
- Extras:
  - Newman (CLI runner) for CI pipelines

### Insomnia (alternative)
- Use-case: clean UI, good for REST/GraphQL workflows

### CLI tools
- curl
- jq (JSON parsing)

---

## Performance Testing

### JMeter
- Use-case: load & performance testing, plugins available

### k6
- Use-case: modern load testing in JavaScript, CI-friendly

---

## Mobile Testing

### Android Studio
- Use-case: emulator, debugging, logcat, APK installs

### Appium
- Use-case: cross-platform mobile automation (Android/iOS)
- Typical requirements:
  - Node.js
  - Java JDK
  - Android Studio (Android SDK)
  - Xcode (macOS only, for iOS)

---

## Databases & Data Tools

### SQL Clients
- DBeaver (multi-db)
- Oracle SQL Developer (Oracle)
- Azure Data Studio / SSMS (SQL Server)

### Useful CLIs
- psql (Postgres)
- mysql client
- sqlite

---

## CI/CD & DevOps

### GitHub Actions
- Use-case: automated test runs on PRs, scheduled runs, publishing reports

### Docker
- Use-case: reproducible environments, running test dependencies locally (DBs, services)

---

## Reporting & Test Management

### Test Reporting
- Allure Report
- Playwright HTML Report
- JUnit XML output (for CI integration)

### Test Management (org dependent)
- Jira + Zephyr / Xray
- Azure DevOps Test Plans

---

## Nice-to-Have Utilities

- Fiddler / Charles Proxy (traffic inspection)
- Browser DevTools mastery
- WSL2 (Windows) for Linux-like dev/test environment
- .env management tools (direnv optional)

---

## Verification Checklist

After installation, verify:

- `git --version`
- `node -v` and `npm -v` (if using Node)
- `python --version` and `pip --version` (if using Python)
- `docker --version` (if installed)
- Playwright: run a quick init and test
- Postman: import a sample collection and hit a public API

---

## Docs

Platform/stack-specific guides live in `/docs`:
- Windows setup
- macOS setup
- Linux setup
- Browser drivers
- Playwright setup
- Selenium setup
- API testing setup
- Performance testing setup
- Mobile testing setup
- CI/CD setup
- Troubleshooting

---

## License

MIT (recommended for public sharing), unless you want a more restrictive license.
