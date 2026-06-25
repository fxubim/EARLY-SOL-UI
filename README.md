# ALPHA FEED — frontend

The React app for the ALPHA FEED Solana scanner. Already wired to the live
backend at `https://early-sol.onrender.com/api` (see `PROXY_BASE` in `App.jsx`).

## Deploy to Vercel

1. Put these files in a new GitHub repo (all at the root — no folders).
2. Vercel → **Add New** → **Project** → import the repo.
3. Leave everything default:
   - Framework Preset: **Vite** (auto-detected)
   - Build Command: `npm run build`
   - Output Directory: `dist`
   - Root Directory: `./` (leave as is)
4. **Deploy.**

Open the Vercel URL on your phone — the feeds should go green and live
sub-$100K tokens stream in.

## Files

- `App.jsx` — the whole scanner (single component)
- `main.jsx` — React entry
- `index.html` — page shell (loads `/main.jsx`)
- `vite.config.js`, `package.json` — build setup

## Change the backend URL later

Edit `PROXY_BASE` near the top of `App.jsx`. Leave it `""` to run in demo mode
(DexScreener + pump.fun only, no proxy).

## Not financial advice

Sub-$100K memecoins are extremely risky and most go to zero. Signals reduce —
never remove — rug risk. Only risk what you can afford to lose.
