# WealthFlow — Financial Asset Management

A free responsive personal financial asset management demo created for Wenting Wang. The entire app runs in `index.html` without build steps, dependencies, accounts, APIs, or a paid backend.

## Features
- Financial overview with asset values, allocation donut, illustrative trend, and top positions
- Add, edit, delete, filter, and search manually priced asset holdings
- Record and browse financial transactions (ledger only; does not update holdings automatically)
- Create, update, and track financial goals
- Portfolio analytics, category breakdown, gain/loss relative to entered cost basis
- Context-aware **local rules-based chatbot** that uses portfolio data (not a hosted LLM)
- CSV export and JSON backup/restore
- Responsive mobile / desktop interface, stored locally via browser localStorage

## Deploy to GitHub Pages (free)
1. Create a public GitHub repository, e.g. `wealthflow`.
2. Upload `index.html` to the repository root. (`README.md` is optional.)
3. Navigate to repository **Settings → Pages**.
4. Under **Build and deployment**, choose **Deploy from a branch**, then **main** and **/(root)**. Save.
5. Open `https://YOUR-USERNAME.github.io/wealthflow/` after GitHub finishes deploying.

Or open `index.html` directly in a modern browser to preview.

## Security, data, and limitations
- The initial holdings, prices, transactions, goals, and six-month chart are **fictional examples**.
- Market prices and cost bases are entered manually. There are **no live market feeds**, bank/broker connections, authentication, multi-device sync, or server database.
- Holdings and transactions are separate and recording a transaction does **not** automatically adjust a holding or calculate capital gains.
- Displayed gain/loss compares estimated current values to entered cost basis, not actual investment performance or tax outcomes.
- The six-month performance chart is only an illustrative shape derived from the present portfolio value, **not an actual price history**.
- Data is stored in the browser's localStorage for this site; it is **not encrypted at rest by the app**. Browser data may be cleared, so use JSON backup if needed.
- Public GitHub repositories are not suitable for confidential financial records, account numbers, credentials, or API keys.
- Chatbot answers use deterministic keyword rules and current local portfolio data. No third-party AI API or external data transfer.
- Educational demo only; not financial or investment advice.

## Customize
Edit the `seed` object in `index.html` to change the fictional sample values. Edit the title, brand, or CSS variables near the top for colors and typography.
