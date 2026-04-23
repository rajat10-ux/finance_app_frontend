# 💸 Expense Tracker — Frontend

A fast, single-file HTML frontend for tracking Debit and Credit expenses.

🔗 **Live:** [https://finance-app-frontend-gold-ten.vercel.app](https://finance-app-frontend-gold-ten.vercel.app)

---

## 📁 Structure

```
expense-tracker.html   ← entire app (HTML + CSS + JS in one file)
```

No framework. No build step. No npm. Just open the file.

---

## ✨ What It Does

- **Add expenses** — fill in amount, category (Debit/Credit), description, and date
- **Filter by category** — dropdown to show only Debit or Credit entries
- **Sort by date** — toggle between newest first / oldest first
- **Live totals** — visible total and entry count update after every filter or sort
- **Stat cards** — always shows total debits, total credits, and visible total at a glance

---

## 🛡 Edge Cases Handled

| Scenario | How it's handled |
|----------|-----------------|
| User clicks submit twice | Button disabled while request is in-flight |
| Page refresh | Re-fetches all data from API on every load |
| Slow API response | Skeleton loader shown while fetching |
| API failure | Toast error message, empty state shown in table |
| Missing fields | Inline validation — category, amount, and date are required |
| Date sort API fails | Falls back to client-side sort automatically |

---

## 🎨 UI Components

- **Topbar** — app name + live API connection status dot
- **Stat cards** — visible total, total debits, total credits
- **Add form** — category tab picker, amount, description, date inputs
- **Controls bar** — category filter dropdown, sort toggle, refresh button
- **Expense table** — date, category badge, description, amount columns
- **Toast notifications** — bottom-center success/error messages
- **Loading skeletons** — animated placeholder rows while fetching

---

## 🌐 Deployment

Deployed on **Vercel** — [https://finance-app-frontend-gold-ten.vercel.app](https://finance-app-frontend-gold-ten.vercel.app)

To redeploy after changes:

```bash
npm i -g vercel
vercel --prod
```

---

## 🧰 Tech

- HTML5, CSS3, Vanilla JavaScript (no dependencies)
- Google Fonts — [Outfit](https://fonts.google.com/specimen/Outfit) + [Space Mono](https://fonts.google.com/specimen/Space+Mono)
- Hosted on [Vercel](https://vercel.com)

---
