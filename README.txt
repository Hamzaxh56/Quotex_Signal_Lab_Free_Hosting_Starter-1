QUOTEX SIGNAL LAB — FREE HOSTING STARTER

What this is:
- Android-friendly, static signal dashboard.
- Shows no invented prices. Until a backend exists, the status correctly says market feed unavailable.
- Calls /api/candles with query params symbol, timeframe, market.
- Expects JSON: {"candles":[{"time":"2026-10-23T12:00:00Z","open":1.1,"high":1.2,"low":1.0,"close":1.15}, ...]}
- Requires at least 20 genuine candles. Keep any market-data API key on the backend, never in index.html.
- OTC data must come from a legitimate source that specifically supports the relevant OTC quotes. Normal forex data is not a substitute.

FREE STATIC HOSTING (GitHub Pages):
1. Create/sign in to GitHub and create a public repository.
2. Upload index.html from this folder to the repository root.
3. Open repository Settings -> Pages.
4. Under Build and deployment, choose Deploy from a branch, select main and /(root), then Save.
5. Wait for the published URL shown in Settings -> Pages.

IMPORTANT:
GitHub Pages only hosts the static front end. It does NOT provide /api/candles. For real data you also need a backend endpoint hosted separately (a free tier may have limits or sleep). Until configured, signals remain WAIT and no price is fabricated.
No auto-trading or Quotex login integration is included. Signals are basic EMA/direction rules, not validated AI predictions.
