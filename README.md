# CyberCrawl — Security+ SY0-701

A single-file, browser-based RPG for studying the CompTIA Security+ (SY0-701) exam. Fight your way through 5 domains as enemies, bosses, and interactive labs quiz you on real exam content.

## Play it

Open `index.html` in any modern browser — no build step, no server, no dependencies beyond a Google Fonts CSS import. Everything (game state, spaced-repetition review data, and any saved "lead" info) is stored locally in your browser via `localStorage`; nothing is sent anywhere.

If GitHub Pages is enabled for this repo, it'll also be playable directly at the Pages URL for this repository (since the file is named `index.html`).

## Features

- 5 domain "sectors" mapped to the SY0-701 exam blueprint, each with regular enemies, a boss fight, PBQ-style scenarios, and interactive labs (packet capture analysis, terminal command labs, log review, firewall rule building, and timeline/sequencing exercises)
- Spaced-repetition review system — missed questions come back due for review
- Study Mode and a full 90-question Exam Simulation mode (90 minutes, pass threshold 750/900)
- Normal/Hard difficulty, role specializations, side quests, and prestige tracking

## Tech

Plain HTML/CSS/JS in a single file. No build tooling, no frameworks.
