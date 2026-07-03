# FinTech H5 Demos

<p align="center">
  <img src="https://img.shields.io/badge/Demos-12-blue" alt="12 Demos" />
  <img src="https://img.shields.io/badge/Dependencies-Zero-green" alt="Zero Dependencies" />
  <img src="https://img.shields.io/badge/License-MIT-yellow" alt="License: MIT" />
  <img src="https://img.shields.io/badge/Type-Single_File_HTML-orange" alt="Single File HTML" />
</p>

12 self-contained financial H5 dashboard demos. **Zero dependencies, zero build steps — just open in a browser.**

Each demo is a single `index.html` file with embedded CSS and JavaScript, featuring dark-theme dashboards, responsive layouts, interactive charts, and realistic mock data.

## Demos

| # | Demo | Description | Key Features |
|---|------|-------------|-------------|
| 1 | [Fraud Alert](./fraud-alert/) | Real-time fraud detection dashboard | Alert timeline, risk scoring, geographic heat map |
| 2 | [Loan Application](./loan-application/) | Digital loan application workflow | Multi-step form, document upload, approval tracking |
| 3 | [Risk Assessment](./risk-assessment/) | Enterprise risk scoring dashboard | Radar charts, risk matrix, trend analysis |
| 4 | [Account Management](./account-management/) | Customer account overview | Balance charts, transaction history, KYC status |
| 5 | [Approval Flow](./approval-flow/) | Multi-level approval workflow | Flow visualization, status tracking, delegation |
| 6 | [Customer Profile](./customer-profile/) | 360-degree customer view | Tag cloud, relationship graph, activity timeline |
| 7 | [Data Report](./data-report/) | Business intelligence report | Pivot tables, KPI cards, export options |
| 8 | [Data Visualization](./data-visualization/) | Interactive data charts | 10+ chart types, drill-down, real-time refresh |
| 9 | [Notification Center](./notification-center/) | Multi-channel notification hub | Priority inbox, read status, batch actions |
| 10 | [Supply Chain](./supply-chain/) | Supply chain finance dashboard | Flow diagram, invoice tracking, settlement status |
| 11 | [Wealth Preservation](./wealth-preservation/) | Wealth management overview | Portfolio allocation, performance curves, rebalancing |
| 12 | [API Test](./api-test.html) | API testing utility | Request builder, response viewer, history log |

## Quick Start

```bash
# Clone the repo
git clone https://github.com/yuzhaopeng-up/fintech-h5-demos.git

# Open any demo directly in your browser
open fintech-h5-demos/fraud-alert/index.html

# Or serve with any HTTP server
cd fintech-h5-demos
python -m http.server 8080
# Visit http://localhost:8080/fraud-alert/
```

No `npm install`. No build step. No configuration. Just HTML.

## Features

- **Dark theme** — Professional fintech aesthetic out of the box
- **Mobile responsive** — Works on desktop, tablet, and phone
- **Interactive charts** — Built with lightweight inline SVG/Canvas
- **Mock data included** — Realistic demo data for all dashboards
- **Zero dependencies** — No external CSS/JS libraries required
- **Single file per demo** — Easy to fork, modify, and deploy

## Use Cases

- **Prototyping** — Jump-start your fintech dashboard with a ready-made template
- **Demonstrations** — Show stakeholders what the finished product looks like
- **Learning** — Study how financial dashboards are structured (forms, charts, workflows)
- **Hacking** — Replace mock data with real APIs and ship it

## Customization

To connect to real APIs, find the mock data section in each HTML file and replace:

```javascript
// Before (mock data)
const transactions = [
  { id: 'TXN001', amount: 50000, status: 'completed' },
  ...
];

// After (real API)
const response = await fetch('/api/transactions');
const transactions = await response.json();
```

## Tech Stack

| Component | Technology |
|-----------|-----------|
| Structure | HTML5 Semantic |
| Styling | Inline CSS (Dark Theme) |
| Charts | Inline SVG / Canvas |
| Logic | Vanilla JavaScript (ES6+) |
| Data | Embedded JSON mock data |

## Ecosystem

These demos are part of the **Agent Skill Ecosystem**:

| Repo | Description |
|------|------------|
| [financial-ai-skills](https://github.com/yuzhaopeng-up/financial-ai-skills) | 104 financial AI skills |
| [skill-framework](https://github.com/yuzhaopeng-up/skill-framework) | Skill governance framework & templates |
| [teleagent-skills](https://github.com/yuzhaopeng-up/teleagent-skills) | General business skills |
| [agent-cluster-comm](https://github.com/yuzhaopeng-up/agent-cluster-comm) | Agent cluster communication |
| **fintech-h5-demos** (this repo) | Financial dashboard demos |
| [soe-compliant-office](https://github.com/yuzhaopeng-up/soe-compliant-office) | SOE-compliant office skills (GB/T 9704, audit trail) |

## Contributing

1. Fork this repository
2. Add your own H5 demo (single HTML file, dark theme)
3. Follow the existing naming convention (kebab-case directory)
4. Test in Chrome, Firefox, and Safari
5. Submit a pull request

## License

MIT License — use freely in personal and commercial projects.
