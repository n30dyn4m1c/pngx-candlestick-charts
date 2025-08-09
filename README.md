# 📈 PNGX Candlestick Chart Viewer

A lightweight web app that fetches OHLC data for PNGX-listed equities via the **NUKU API** and renders interactive candlestick charts. Designed for PNG investors, traders, and market watchers who want quick, browser-based access to recent stock data without installing software.

---

## 🧰 Tech Stack

- **Frontend**: Single-file HTML (inline CSS + JS)
- **Charts**: ApexCharts (candlestick)
- **Data Source**: NUKU API (by Christian Augustyn – [GitHub](https://github.com/chrisaugu/pngx-api))
- **Hosting**: GitHub Pages

---

## 🚀 Key Features

- ✅ Static dropdown of PNGX symbols 
- ✅ Date pickers (default last 30 days)
- ✅ Single-symbol OHLC fetch and render
- ✅ Timeout and clear status messages (incl. 503)
- ✅ Proper credits to NUKU API and creator

---

## 📊 Workflow Logic

1. User selects stock symbol from dropdown.
2. User sets start/end dates.
3. Click "Load chart" (or press Enter).
4. App requests `/historicals/{SYMBOL}?start=YYYY-MM-DD&end=YYYY-MM-DD`.
5. Parse to `{x: Date, y: [o,h,l,c]}` and update ApexCharts.
6. Show candle count or errors if empty/unavailable.

---

## 🗂 Included Files

| File         | Description                     |
|--------------|---------------------------------|
| `index.html` | UI, styling, JS, and chart code |

---

## 🛠️ Setup Instructions

1. Create a new public GitHub repo.
2. Add `index.html` (this file) to the repo root.
3. Commit and push.
4. In GitHub: Settings → Pages → Deploy from branch → `main` / root.
5. Open the Pages URL and select a stock + dates.

---

## 📝 License & Acknowledgments

- © 2025 **Neo Malesa** – Developer of this frontend.
- **NUKU API** by Chris Augu ([GitHub Repo](https://github.com/chrisaugu/pngx-api)) – Data provider.
- Data accuracy depends on PNGX/NUKU API uptime; use responsibly.

---
