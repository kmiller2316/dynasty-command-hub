# 🏆 Dynasty Command Hub

A single-file, zero-cost dynasty fantasy football command center. Enter your Sleeper username, pick a league, and get roster grades, trade tools, draft prep, and league-wide manager scouting — all computed in your browser with **no API key and no paid services**.

**▶ Live app: https://kmiller2316.github.io/dynasty-command-hub/**

Open it on your phone in Safari → **Share → Add to Home Screen** to install it as an app.

---

## Features

| Tab | What it does |
|-----|--------------|
| 📋 **Roster** | Your full roster grouped by position, with FantasyCalc values, ages, and value bars. |
| 💎 **Assets** | Draft picks you own vs. traded away, plus a league-wide roster-value comparison. |
| 📅 **Weekly** | Week-by-week matchups, results, and season standings. |
| 🏛️ **Dynasty Value** | Your roster ranked by dynasty value, plus an automatic **A–F roster grade report** (per position + overall, age curve, strengths/weaknesses, 12-month outlook). |
| ⚖️ **Trade Grader** | Build any trade by searching players or picks. Toggle **Lowball / Fair / Overpay** to shift the verdict, and exclude any piece from the estimate with one tap. |
| 📨 **Trade Finder** | **Buy** any player (finds the owner and builds a fair offer from your assets) or **Sell** one of yours (ranks likely buyers and what they'd send back). Filter returns to **picks only** or **youth**, target a specific team or anyone, and set untouchables. |
| 🎯 **Draft Center** | Projected draft order, your pick slots, best-available players, and a rule-based mock draft simulator. |
| 👤 **Managers** | League-wide scouting: win-now index, age profile, positional bias, pick capital, roster construction, and matchup luck for every team — with a legend and trade-fit flags. |
| 📊 **GM Grades** | Report card grading every manager on **drafting** (picks vs. draft-slot expectation), **trading** (net value across all deals), and **waivers** (value of pickups still rostered). |
| 🏅 **Commissioner** | Reverse-points draft order, projected final order, trade log, and full-season results. |

## How it works

All analysis runs **client-side with rule-based engines** — no LLM calls, no server, no cost per use.

- **Sleeper API** (free, no key) — leagues, rosters, users, matchups, traded picks.
- **FantasyCalc API** (free, no key) — current dynasty player and draft-pick values, matched to your league's format (1QB / Superflex, PPR, team count).
- **Static pick-value chart** — bundled in the file for draft-pick valuation.

Nothing is stored anywhere but your own browser's `localStorage` (used only to remember recently loaded leagues).

## Usage

1. Open the [live app](https://kmiller2316.github.io/dynasty-command-hub/).
2. Enter your Sleeper username and season, then **🔍 Find My Leagues**.
3. Pick a league from the list. Everything loads automatically.

No account, no sign-up, no API key.

## Tech

- One `index.html` file — vanilla HTML, CSS, and JavaScript.
- No frameworks, no build step, no dependencies, no bundler.
- Works offline after first load, except for live Sleeper / FantasyCalc data fetches.
- Mobile-first responsive layout with iOS home-screen (PWA-style) support.

## Contributing

Changes go through a pull request against `master` — direct pushes to the default branch are not accepted. Open a PR and it can be reviewed and merged.

---

*Powered by [Sleeper](https://sleeper.com) + [FantasyCalc](https://fantasycalc.com). Not affiliated with either.*
