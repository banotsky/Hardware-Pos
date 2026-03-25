# 🏪 HardwareStore ERP — Offline PWA

A **simple, fast, fully offline ERP web app** for hardware stores. Works 100% without internet after first load. All data stored locally using **IndexedDB**.

---

## 🔐 Login Credentials

| Field | Default Value |
|-------|--------------|
| Username | `admin` |
| Password | `admin` |

> You can change the password after login via **Change Password** in the user menu.

---

## 🚀 Features

### 🔐 Authentication
- Login screen with username/password
- Session persists for 8 hours
- Change password option after login
- Sign out button

### 🔍 Global Search
- Searches across **all data** simultaneously: Products, Sales, Purchases
- Click any result to jump directly to that section
- Highlighted match text

### 📊 Dashboard
- Date range filter (Today / This Week / This Month / All Time / Custom)
- Stats: Sales Revenue, Products, Low Stock, Transactions
- Low stock alerts list
- Searchable recent transactions list

### 📦 Inventory
- Add/Edit/Delete products
- **Advanced Search**: name, category, price range, stock range, stock status
- Category filter pills with counts
- Sort by: Name, Price, Stock
- Low stock badges

### 🛒 POS (Point of Sale)
- Category filter for products
- Product search
- Cart with quantity controls
- Auto-compute total, payment, change
- Full receipt modal on sale completion

### 📥 Purchases (Stock In)
- **Advanced Filters**: date range, product name, cost range, category, sort
- Auto-updates inventory on stock-in
- Total cost summary

### 📋 Reports
- **Advanced Filters**: date range, amount range, sort order
- Quick date shortcuts: Today, Yesterday, This Week, This Month, All Time
- Summary stats (Total Sales, Transactions, Items Sold)
- Searchable transaction list
- **Export to CSV** (filtered results)

---

## 📱 How to Run Locally

### Option 1 — Open directly (basic)
Double-click `index.html` in Chrome or Edge.

### Option 2 — Local server (recommended, full PWA)
```bash
# Python
python -m http.server 8080
# Open: http://localhost:8080

# Node.js
npx serve .
# Open the URL shown

# VS Code Live Server
# Right-click index.html → Open with Live Server
```

### Option 3 — Install as Android PWA
1. Open in **Chrome** on Android
2. Tap **📲 Install App** button in top bar
3. Or Chrome menu → "Add to Home screen"

---

## 🗂️ File Structure

```
index.html        ← Complete app (Vue 3, all screens)
manifest.json     ← PWA manifest
sw.js             ← Service Worker
icons/
  icon-192.png    ← PWA icon
  icon-512.png    ← PWA icon
README.md
```

---

## 💾 Data Storage

- **IndexedDB** — all products, sales, purchases
- **localStorage** — user credentials + session
- **Nothing sent to any server** — 100% private, offline-first

---

## 🎨 UI Theme

- **Full glassmorphism** — transparent cards with blur effects
- **Animated background** — subtle floating glow orbs
- **Dark navy** base with amber accent color
- **Mobile-first** — works on Android, iOS, desktop

---

*Built with ❤️ for small hardware store owners. Simple. Fast. Offline.*
