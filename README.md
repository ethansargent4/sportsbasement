# Sports Basement — AI Trip Planner

The AI-native gear advisor. Tell us where you're going and what you've got. We build the kit you actually need.

## Concept

A reimagining of [sportsbasement.com](https://www.sportsbasement.com/) where the primary interaction is conversational: describe your trip in plain English, list what you already own, set a budget, and get back a personalized gear list — categorized into Essentials, Recommended, and Nice-to-have, each with three price tiers and a one-line "why."

## Stack

Pure HTML / CSS / vanilla JS. Single static file. Tiny Node static server for Railway.

## Local

\`\`\`bash
node server.js
# open http://localhost:3000
\`\`\`

## Deploy (Railway)

Push to GitHub, then in Railway dashboard → New Project → Deploy from GitHub Repo → pick this repo. Railway uses Nixpacks to detect Node and runs \`node server.js\`.

## Features

- **Natural-language trip parser** — extracts activity, location, duration, weather conditions, experience level, and items you already own
- **Personalized kit builder** — 9 activities × 3 buckets × 3 tiers, automatic budget fitting
- **AI floor crew chat** — floating "ask the floor crew" affordance with mock conversational responses
- **Refine loop** — natural-language follow-ups
- **Used + consignment** — vibe selector pulls used inventory first
- **Streaming "thinking" UI** — shows reasoning live before results render
