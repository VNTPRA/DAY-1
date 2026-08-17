# 💰 Money Manager

A simple, self-contained personal money management app — all in a **single HTML file** with no external dependencies. Track your income and expenses, see your balance at a glance, and keep your data on your own device.

## ✨ full 
Features

- **Live dashboard** – Total Balance, Total Income, and Total Expenses, recalculated instantly as you add or delete entries.
- **Add transactions** – Enter a description, amount, and type (Income or Expense), with an optional category (Food, Transport, Rent, Salary, Shopping, Other).
- **Smart rows** – Income shows in green, expenses in red, each with the date/time it was added.
- **Filter & search** – Filter the list by category and use the search box to find entries by description.
- **Delete** – Remove any transaction with one click.
- **Input validation** – Friendly error messages block invalid input (empty description, missing/zero/negative amounts).
- **Persistent storage** – Your transactions are saved to `localStorage` and survive page reloads.

## 📖 Usage

1. **Open the app** — just double-click `MoneyManagerApp.html` and it runs in any modern browser. No install, no server, no build step.
2. **Add a transaction** — fill in the description and amount, pick Income or Expense (and an optional category), then click **Add Transaction**.
3. **Review your dashboard** — the three summary cards at the top update automatically.
4. **Manage your list** — use the category filter or search box to narrow things down, and hit the **Delete** button on any row to remove it.
5. **Come back later** — your data is still there, since everything is stored locally in your browser.

## ⚙️ How it works

- Pure **HTML + CSS + JavaScript** in one file — no frameworks, no CDNs, no network calls.
- Transactions are kept in memory and mirrored to `localStorage` under a single key so the page state persists.
- Amounts are formatted as USD (e.g. `$1,234.56`).

## 🔌 Customization (quick ideas)

- **Change currency** – the formatter is a single `formatCurrency()` function near the top of the script; swap the locale/currency there (e.g. `ZAR` for South African Rand).
- **Add categories** – find the `<select>` options in the form and the array used by the filter; add or remove entries freely.
- **Start fresh** – clear your browser's local storage for the site, or reset via your browser's site-data tools.

## 🗂 Files

| File | Purpose |
| --- | --- |
| `MoneyManagerApp.html` | The entire application (UI, styles, and logic). |

## 📄 License

Free to use and modify for personal or commercial projects.

