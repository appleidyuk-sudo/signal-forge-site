# SignalForge Deep Dive — Screenshot Requirements

All screenshots should be taken on an **iPhone 17 Pro simulator (iOS 26.2)** with the app populated with sample stocks (at least 5-8 stocks with positions/cost basis, plus a few watchlist-only). Save each screenshot as a PNG to `signal-forge-site/screenshots/` using the filename listed below.

The deep-dive.html has placeholder `<div>` elements with matching `id` attributes (e.g., `id="ss-home-full"`). Once screenshots are captured, replace each placeholder with an `<img>` tag pointing to the file.

---

## How to Insert Screenshots

For each screenshot below, find the matching `<div class="screenshot" id="ss-XXXX">` in `deep-dive.html` and replace it with:

```html
<div class="screenshot" id="ss-XXXX">
  <img src="screenshots/FILENAME.png" alt="DESCRIPTION">
</div>
```

---

## Screenshot List

### HOME SCREEN (Section: #home)

| # | Filename | Element ID | What to Capture |
|---|----------|-----------|-----------------|
| 1 | `home-full.png` | `ss-home-full` | Full Home screen showing header (logos, version, market status pill), channel bar, position value card, signal count cards, and top pick. Scroll position: top. |
| 2 | `home-channels.png` | `ss-home-channels` | Close crop of the channel bar with one channel selected (highlighted in blue). Show at least 4-5 channel buttons visible. |
| 3 | `home-position.png` | `ss-home-position` | Close crop of the Position Value card showing: total value, P&L (green or red), daily P&L, cost basis, and last update time. |
| 4 | `home-toppick.png` | `ss-home-toppick` | Top Pick card in expanded state showing convergence score, entry/target/stop prices, and the criteria button. If possible, show additional suggestions expanded below. |
| 5 | `home-performance.png` | `ss-home-performance` | Performance History sheet (tap the position value card to open it). Show the line chart with SPY benchmark toggled ON, with the 1M timeframe selected. |
| 6 | `home-leaderboard.png` | `ss-home-leaderboard` | Leaderboard sheet (tap trophy icon). Show the rankings list with a metric selected. |

### WATCHLIST / POSITIONS (Section: #watchlist)

| # | Filename | Element ID | What to Capture |
|---|----------|-----------|-----------------|
| 7 | `watchlist-full.png` | `ss-watchlist-full` | Watchlist screen in **Concise** view showing the toggle (set to Positions), column headers, and several stock rows with signal badges and P&L. |
| 8 | `watchlist-buttons.png` | `ss-watchlist-buttons` | Close crop of the watchlist header showing all action buttons (options overview, bubble chart, insights, help, add). |
| 9 | `watchlist-expanded.png` | `ss-watchlist-expanded` | Watchlist in **Expanded** view showing 2-3 full signal cards with convergence scores and indicator details. |
| 10 | `watchlist-add.png` | `ss-watchlist-add` | Add Stock sheet with fields partially filled in (e.g., symbol "NVDA", quantity "100", avg cost "120.50", Buy selected). |
| 11 | `watchlist-bubble.png` | `ss-watchlist-bubble` | Bubble Chart sheet showing stocks plotted as colored bubbles on the momentum/signal grid. |
| 12 | `watchlist-insights.png` | `ss-watchlist-insights` | Portfolio Insights sheet — News tab showing 3-4 articles with sentiment badges (Bullish/Bearish/Neutral). |

### SECTOR HEATMAP (Section: #heatmap)

| # | Filename | Element ID | What to Capture |
|---|----------|-----------|-----------------|
| 13 | `heatmap-full.png` | `ss-heatmap-full` | Full Heatmap screen in Treemap view showing multiple sectors with colored tiles. Ensure at least 3 sectors are visible with stock labels. |
| 14 | `heatmap-risk.png` | `ss-heatmap-risk` | Heatmap in Risk Analysis mode showing the donut chart, concentration warnings, and/or correlation flags. |

### RESEARCH (Section: #research)

| # | Filename | Element ID | What to Capture |
|---|----------|-----------|-----------------|
| 15 | `research-full.png` | `ss-research-full` | Research screen showing the mode picker buttons (Compare, Discover, Explorer, Showdown) at the top. |
| 16 | `research-compare.png` | `ss-research-compare` | Compare mode with 3-4 stocks overlaid on a normalized performance chart. Include the legend. |
| 17 | `research-discover.png` | `ss-research-discover` | Discover mode showing the universe picker (e.g., S&P 100 selected) and a results table with convergence scores. |
| 18 | `research-explorer.png` | `ss-research-explorer` | Explorer mode with a preset filter applied (e.g., "Oversold Bounces") and filtered results visible. |
| 19 | `research-showdown.png` | `ss-research-showdown` | Showdown sub-tab comparing two indicators with results table visible. |
| 20 | `research-deepdive.png` | `ss-research-deepdive` | Deep Dive sheet — **Technicals** tab showing the signal summary card and the interactive chart with Bollinger Bands. |
| 21 | `research-deepdive-fundamentals.png` | `ss-research-deepdive-fundamentals` | Deep Dive sheet — **Fundamentals** tab showing company profile, analyst consensus, and competitors. |
| 22 | `research-chart.png` | `ss-research-chart` | Expanded chart view (full-screen) showing candlesticks with Bollinger Bands, volume bars, and at least one overlay (EMA or SuperTrend). |
| 23 | `research-optionchain.png` | `ss-research-optionchain` | Option chain view showing calls/puts with an expiration selected, plus at least one Greek butterfly chart visible. |
| 24 | `research-ivhv.png` | `ss-research-ivhv` | IV/HV analysis chart and/or probability distribution view. Show the dual-line IV vs HV chart if possible. |

### SIMULATOR (Section: #simulator)

| # | Filename | Element ID | What to Capture |
|---|----------|-----------|-----------------|
| 25 | `simulator-full.png` | `ss-simulator-full` | Full Simulator screen showing the auto-trade controls, grand total bar, and at least 2-3 active ghost trades. |
| 26 | `simulator-equity.png` | `ss-simulator-equity` | Equity curve chart expanded, with the 3M or ALL timeframe selected. |
| 27 | `simulator-trades.png` | `ss-simulator-trades` | Close crop of 2-3 active ghost trade cards showing symbol, entry price, current P&L (mix of green and red), and days held. |

### OPTIONFLOW (Section: #optionflow)

| # | Filename | Element ID | What to Capture |
|---|----------|-----------|-----------------|
| 28 | `optionflow-full.png` | `ss-optionflow-full` | Full OptionFlow dashboard showing KPI grid and at least 2 active positions with strategy pills. |
| 29 | `optionflow-record.png` | `ss-optionflow-record` | Record Trade sheet with a symbol entered and the option chain loaded (showing expiration pills and strike picker). |
| 30 | `optionflow-multileg.png` | `ss-optionflow-multileg` | Strategy Builder sheet for a multi-leg trade (e.g., Iron Condor or Call Spread) showing multiple legs. |
| 31 | `optionflow-position.png` | `ss-optionflow-position` | Close crop of an active position card showing strategy pill, underlying/strike, DTE badge, ROC%, and roll badge (if visible). |
| 32 | `optionflow-roll.png` | `ss-optionflow-roll` | Roll Advisor sheet showing current position and suggested roll targets. |
| 33 | `optionflow-calendar.png` | `ss-optionflow-calendar` | Income Calendar sheet showing the calendar grid and/or trailing 12-month income chart. |

### SETTINGS (Section: #settings)

| # | Filename | Element ID | What to Capture |
|---|----------|-----------|-----------------|
| 34 | `settings-full.png` | `ss-settings-full` | Full Settings panel showing all sections (biometric lock, darkness slider, refresh interval, notifications, etc.). May need 2 screenshots if it scrolls — capture top half. |
| 35 | `settings-thresholds.png` | `ss-settings-thresholds` | Close crop of the signal threshold sliders (buy threshold and sell threshold). |

---

## Total: 35 screenshots

## Directory Setup

Before capturing, create the screenshots directory:
```bash
mkdir -p /Users/toddc/DHCbot/signal-forge-site/screenshots
```

## Notes for the Screenshot Agent

- Use the **iPhone 17 Pro** simulator (iOS 26.2)
- Build target: `xcodebuild -project DHCbot.xcodeproj -scheme DHCbot -destination 'platform=iOS Simulator,name=iPhone 17 Pro' build`
- The app needs sample data to look good. Add at least 5-8 stocks with positions (e.g., AAPL, MSFT, NVDA, GOOGL, AMZN, TSLA, META, JPM)
- For OptionFlow screenshots, record a few sample option trades first
- For Simulator screenshots, create a few ghost trades first
- Capture at a standard resolution — the website will scale images responsively
- Dark mode is the default and correct appearance
- Use `xcrun simctl io booted screenshot <path>` to capture screenshots
