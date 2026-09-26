# Wispr Flow case study

A two-part product case study for Wispr Flow, built by Angad Gunbharit.

**1. Who Flow Is For (`icp-scan.html`)** — an ICP scan of 124 public signals about Flow: 50 App Store reviews across five countries, all 21 G2 reviews, and 53 Hacker News comments. Each is hand-coded for persona, job, sentiment and themes.

Key findings:
- Knowledge workers and execs were 22 of 24 positive, with no negatives.
- 13 of 21 developer comments were about building or switching to a Flow alternative.
- Only 4 of 28 negative signals were about accuracy. Most were about price, privacy or switching.
- People dictating AI prompts were 11 of 12 positive, and no Wispr page speaks to them.

**2. Flow Prompt Mode (`prompt-mode.html`)** — a prototype of the first experiment the scan suggests. When Flow sees you're dictating into an AI app, it cleans your speech into a structured prompt instead of a short message, keeping every constraint you said. The message cleanup shown is a simulation for comparison, not Wispr's model.

## Data

`flow_signals.csv` holds all 124 coded signals. Columns: `id, source, rating, sentiment, persona, job, themes, note`. Themes are semicolon-separated.

## Limits

This is directional. App Store pages surface their most helpful reviews first, which skews positive. Hacker News skews toward developers. Reddit wasn't reachable for this scan, and Trustpilot has removed Wispr's profile. All coding was done by one person.

## Running it

Static HTML with no build step. Open `index.html`, or serve the folder with GitHub Pages.
