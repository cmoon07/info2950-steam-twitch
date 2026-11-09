# Game Lifecycles on Steam and Twitch

INFO 2950 (Intro to Data Science) project at Cornell University, Fall 2026
Suzie Ahn and Claire Moon

## Research questions
1. In the first 12 months after a game launches on Steam, how much of its launch-peak player base and Twitch audience does it keep? Does Twitch interest fade faster than Steam interest?
2. Do multiplayer and free-to-play games keep their players and viewers longer than other games?

## Data
We built a 347-game dataset by merging monthly Steam player counts (612K records) with Twitch top-200 viewership and Steam store metadata, matching titles through name normalization and hand-verified aliases. See `datasets/raw/README.md` for sources.

## Repository layout
- `notebooks/phase2_eda_preregistration.ipynb`: data cleaning, exploratory analysis, and preregistered hypotheses
- `datasets/clean/`: analysis-ready files (one row per game; one row per game per month)

## Reproducing
1. Download the raw files listed in `datasets/raw/README.md` into `datasets/raw/`.
2. Run the notebooks in `notebooks/` from top to bottom. The Google Drive mount only runs in Colab.
3. Intermediate files (e.g., steam_monthly_clean.csv, 57 MB) aren’t included; the cleaning notebook recreates them from the raw data.

## Status
Phase II (EDA and preregistration) is complete. The analysis and results will be added in Phase III.
