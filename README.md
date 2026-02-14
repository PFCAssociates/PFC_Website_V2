# demorepo4

A GitHub Pages deployment framework with automatic version polling, auto-refresh, and Google Apps Script (GAS) embedding support.

**Live site:** [ShadowAISolutions.github.io/demorepo4](https://ShadowAISolutions.github.io/demorepo4)

## How It Works

### Auto-Refresh via Version Polling
Every hosted page polls a lightweight `.version.txt` file every 10 seconds. When a new version is deployed, the page detects the mismatch and auto-reloads — showing a green "Website Ready" splash with audio feedback.

### CI/CD Auto-Merge Flow
1. Push to a `claude/*` branch
2. GitHub Actions automatically merges into `main`, deploys to GitHub Pages, and cleans up the branch
3. No pull requests needed — the workflow handles everything

### GAS Embedding Architecture
Google Apps Script projects are embedded as iframes in GitHub Pages. The framework handles:
- Automatic GAS deployment via `doPost` when `.gs` files change
- "Code Ready" blue splash on GAS updates (client-side polling)
- Google Sign-In from the parent page (stable OAuth origin)

## Project Structure

```
demorepo4/
├── httpsdocs/                  # Deployed to GitHub Pages
│   ├── index.html              # Live landing page
│   ├── index.version.txt       # Version file for auto-refresh
│   └── sounds/                 # Audio feedback files
├── autoUpdateTemplateFiles/    # Template for new pages
├── .github/workflows/          # CI/CD pipeline
├── ARCHITECTURE.md             # System diagram (Mermaid)
├── CHANGELOG.md                # Version history
├── CLAUDE.md                   # Developer instructions
├── STATUS.md                   # Project status dashboard
└── LICENSE                     # Proprietary license
```

## Documentation

| Document | Description |
|----------|-------------|
| [ARCHITECTURE.md](ARCHITECTURE.md) | Visual system diagram (Mermaid) |
| [CLAUDE.md](CLAUDE.md) | Developer instructions and conventions |
| [CHANGELOG.md](CHANGELOG.md) | Version history |
| [STATUS.md](STATUS.md) | Current project status and versions |

Developed by: ShadowAISolutions
