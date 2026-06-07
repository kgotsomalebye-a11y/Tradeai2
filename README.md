# TradeAI Dashboard — Setup Instructions

## What's included
- `index.html` — Main dashboard (open this in your browser)
- `manifest.json` — PWA manifest for phone installation
- `sw.js` — Service worker for offline support

## How to use on your computer
1. Open `index.html` in Chrome or Edge
2. Use the market buttons at the top to switch between instruments
3. Use the timeframe buttons to switch between 15m, 30m, 1H, 4H
4. Press the green refresh button to update analysis

## How to install on your phone (Android)
1. Host these files on any web server (see hosting options below)
2. Open the URL in Chrome on your Android phone
3. Tap the "Install" banner that appears, or tap the 3-dot menu → "Add to Home Screen"
4. The app will appear on your home screen like a native app

## How to install on iPhone (iOS)
1. Host these files on a web server
2. Open the URL in Safari on your iPhone
3. Tap the Share button (box with arrow pointing up)
4. Scroll down and tap "Add to Home Screen"
5. Tap "Add" — the app appears on your home screen

## Free hosting options
### Option 1 — GitHub Pages (recommended, free)
1. Create a free account at github.com
2. Create a new repository called "tradeai"
3. Upload all three files (index.html, manifest.json, sw.js)
4. Go to Settings → Pages → Select "main" branch → Save
5. Your dashboard will be live at: https://yourusername.github.io/tradeai

### Option 2 — Netlify (easiest, free)
1. Go to netlify.com and create a free account
2. Drag and drop your folder onto the Netlify dashboard
3. Get an instant live URL you can access from anywhere

### Option 3 — Vercel (free)
1. Go to vercel.com and create a free account
2. Import your files and deploy instantly

## Markets included
Commodities: XAUUSD (Gold), XAGUSD (Silver), USOIL (WTI Crude)
Forex: EURUSD, GBPUSD, USDJPY, AUDUSD, USDCAD

## Timeframes
15 minutes, 30 minutes, 1 Hour, 4 Hours

## Note on live data
The current version uses simulated market data for demonstration.
To connect live TradingView data, you would need to set up webhook
alerts from TradingView that update the dashboard in real time.
This can be done by connecting a backend server to receive the
TradingView webhook signals we set up earlier.
