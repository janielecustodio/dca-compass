# DCA Compass 📡

**Dollar-Cost Averaging Portfolio Simulator — USA & Brazil**

Live site: `https://<your-github-username>.github.io/dca-compass`

Supports US ETFs, Brazilian B3 stocks, dual USD/BRL returns, FX analysis, and technical signals — all powered by Yahoo Finance data, no backend required.

---

## 🚀 One-time setup (~3 minutes)

### Step 1 — Create the GitHub repository

Go to [github.com/new](https://github.com/new) and create a **public** repository named:
```
dca-compass
```
Leave it empty (no README, no .gitignore). Click **Create repository**.

### Step 2 — Push this code

Open a terminal in this folder and run:

```bash
git init
git add .
git commit -m "Initial deploy"
git branch -M main
git remote add origin https://github.com/<YOUR_USERNAME>/dca-compass.git
git push -u origin main
```

> Replace `<YOUR_USERNAME>` with your actual GitHub username.

### Step 3 — Enable GitHub Pages

1. Go to your repo on GitHub
2. Click **Settings** → **Pages** (left sidebar)
3. Under **Source**, select **GitHub Actions**
4. Click **Save**

GitHub will automatically run the deploy workflow. In about 60 seconds your app will be live at:

```
https://<YOUR_USERNAME>.github.io/dca-compass
```

---

## 🔄 Updating the app

Any time you push changes to `main`, GitHub Actions redeploys automatically:

```bash
git add .
git commit -m "Update"
git push
```

---

## 📁 File structure

```
dca-compass/
├── index.html              ← The entire app (self-contained)
├── README.md
└── .github/
    └── workflows/
        └── deploy.yml      ← Auto-deploy on push
```

---

## 🛠 Features

- **Portfolio Builder** — any Yahoo Finance ticker with custom weights
- **Presets** — SPY+EWZ, US 60/40, BOVA11 only, QQQ+BOVA11, Global Mix, Brazil Focus
- **DCA Periods** — 1W / 2W / 1M / 2M / 3M / 6M
- **Dual Currency** — invest in USD, BRL, or both; see returns in both
- **FX Analysis** — USD/BRL chart + currency impact on returns
- **Technical Signals** — SMA 20/50, RSI, volatility, DCA entry quality
- **History Table** — full timeline with per-date values and FX rates
- **Per-Asset Breakdown** — individual returns, shares, purchases

---

## 📊 Supported tickers

| Market | Examples |
|--------|---------|
| US ETFs | SPY, QQQ, IVV, VTI, GLD, BND, EWZ |
| Brazil ETFs (USD) | EWZ, BRZU |
| Brazil B3 | BOVA11.SA, PETR4.SA, VALE3.SA, ITUB4.SA, SMAL11.SA |
| FX | BRL=X (auto-fetched) |

Any valid Yahoo Finance ticker works.

---

*Data sourced from Yahoo Finance public API. For educational purposes only — not financial advice.*
