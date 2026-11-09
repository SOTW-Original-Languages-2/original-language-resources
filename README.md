# SOTW Original Language Resources | Part 2

This is the **public static resource foundation** for Bible word-study evidence from **Proverbs through Revelation**. It holds the second half of an owner-verified two-foundation release. The existing Part 1 foundation contains **Genesis through Psalms** and the **one shared Hebrew/Greek Strong’s lexical library**.

- **Part 2 foundation:** https://github.com/SOTW-Original-Languages-2/original-language-resources
- **Part 1 and shared lexicon:** https://github.com/SOTW-Original-Languages/original-language-resources
- **Public route map:** [`study-data/v1/route-map.json`](study-data/v1/route-map.json)
- **Resource contract:** [`study-data/v1/contract.json`](study-data/v1/contract.json)
- **SHA-256 file manifest:** [`study-data/v1/manifest.json`](study-data/v1/manifest.json)
- **Source credits and rights:** [`study-data/v1/attribution.json`](study-data/v1/attribution.json) and [`RIGHTS_AND_ATTRIBUTION.md`](RIGHTS_AND_ATTRIBUTION.md)

## Retrieval

Get `study-data/v1/route-map.json` from either foundation and use `site_roots[book.repo_id].planned_pages_base` to resolve the correct book. The chapter endpoint is `study-data/v1/chapters/{BOOK}/{NN}.json` and has verse-keyed evidence for KJV 1769, BSB, ASV 1901, and Webster Bible 1833. To retrieve full Strong’s entries, follow `lexicon_repository_id` to Part 1 and fetch the appropriate 250-entry lexical shard.

A chapter file contains accepted **word-link evidence**, **not** the English Bible verse text, and does not assert that native KJV tagged-word ordinals or BSB source rows are English text offsets. The ASV/Webster derived target offsets retain their accepted evidence status. The reader must separately load edition-specific Bible text, English Webster 1828 dictionary entries, and source-specific commentary.

This foundation is a resource endpoint, **not** the future Bible-reading UI. The separate Part 1 Word Study demo remains a demonstration.

## Publication and integrity

JSON is served uncompressed as normal static files; the ZIP upload packs are only for owner transport. Public availability must be verified after GitHub Pages publication. Check every fetched file against the SHA-256 list in `study-data/v1/manifest.json`. The manifest does not hash itself. See the owner's private corrected upload kit for installation instructions and recovery.
