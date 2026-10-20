# SG PSI & Weather Update

Problem Set 5 agent page (MGMT 6110): a Zapier agent that emails me Singapore's official 24-hour PSI and PM2.5 for five regions, plus the weather, at 00:00, 06:00, 12:00 and 18:00 SGT, using NEA's public data on data.gov.sg.

- `index.html`: the PS5 page (agent card, runs checked against Zap history, tricky case and fix, map, Q1, collaboration log, reflection)
- `sg-weather-watch.html`: my earlier one-trigger, one-action attempt (archived; it never fired)
- `board.html`: our group's Week 7 map board

A static site with no build step. The Zap-history JSON is kept off GitHub (`*.json` in `.gitignore`).

## Editing the write-ups on the live page

1. Open **https://ps5-weather-agent.vercel.app/?edit**. Every write-up block gets a dashed outline; click into it and type.
2. Press **Save to GitHub**. The first time, paste a GitHub token (see below). The page commits the new `index.html` to this repository, and Vercel redeploys it in about 30 seconds.
3. **Download page** gives you the edited `index.html` instead, if you would rather upload it yourself. **Discard changes** reloads the page.

Visitors without `?edit` never see the editing controls.

### Making the token (once)

GitHub → Settings → Developer settings → Personal access tokens → **Fine-grained tokens** → Generate new token:
- Repository access: **Only select repositories** → `kevinch10/ps5-weather-agent`
- Permissions → Repository permissions → **Contents: Read and write**
- Expiration: a short one, e.g. 7 days

The token is kept only in your own browser (untick "Remember on this device" to keep it for one save only, or press **Forget token**). It is sent only to `api.github.com`.
