# World Cup 2026 TikTok Creators — Open Dataset

Per-nation profile of TikTok creators across the **48 nations qualified for the
2026 FIFA World Cup**, from Crawlora's `creators_search` dataset (≈3.33M
discoverable creators), **June 2026 snapshot**. Aggregate rollups only — counts
and rates by nation, never individual creators.

📊 **Study:** https://crawlora.net/blog/world-cup-creators-2026

## Coverage

A creator's country comes primarily from TikTok's own account region (with a
best-effort flag-emoji / place-name bio fallback) and is present on ~7.7% of the
dataset. We therefore measure the **170,551** qualified-nation creators who carry
a detected country, and rank the **26 of 48** nations with at least 300 of them.
Every figure reads as "among established creators with a known country," and
country reflects **account region, not nationality**.

## Files

- `data/world-cup-creators-2026.csv` — one row per measurable nation.
- `data/world-cup-creators-2026.json` — the same data plus headline aggregates and the list of unmeasurable nations.

### Columns

| column | meaning |
|---|---|
| `nation`, `code`, `confederation` | nation name, ISO code (England + Scotland share `gb`), FIFA confederation |
| `creators` | creators with this detected country |
| `verified_pct` | share carrying a verified badge |
| `contact_pct` | share listing a business-contact email in bio |
| `reach_100k_pct`, `reach_1m_pct` | share with ≥100k / ≥1M followers |
| `median_followers` | median follower count |
| `micro_pct` | share in the 10k–100k micro tier |
| `english_pct` | share whose posting language is English |
| `bookable_micro` | micro-tier creators that also list a contact email |

## License

[Creative Commons Attribution 4.0 International (CC BY 4.0)](LICENSE). Please
attribute **Crawlora** and link back to the study.

## Source

Generated from the Crawlora TikTok creators API (`/datasets/creators/search`).
Learn more: https://crawlora.net
