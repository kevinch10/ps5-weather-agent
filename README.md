# SG PSI & Weather Update

Problem Set 5 agent page (MGMT 6110): a Zapier agent that emails me Singapore's official 24-hour PSI and PM2.5 for five regions, plus the weather, at 00:00, 06:00, 12:00 and 18:00 SGT, using NEA's public data on data.gov.sg.

- `index.html`: the PS5 page (agent card, runs checked against Zap history, tricky case and fix, map, Q1, collaboration log, reflection)
- `sg-weather-watch.html`: my earlier one-trigger, one-action attempt (archived; it never fired)
- `board.html`: our group's Week 7 map board

A static site with no build step. The Zap-history JSON is kept off GitHub (`*.json` in `.gitignore`).
