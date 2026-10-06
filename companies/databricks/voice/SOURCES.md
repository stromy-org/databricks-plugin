# Sources — Databricks voice (captured 2026-10-06)

Read (via WebFetch/WebSearch; page-to-markdown summarizer, so quotes were copied
from its returned text):

1. https://www.databricks.com/company/about-us — mission, platform sentence (verbatim anchors).
2. https://www.databricks.com/ — hero "One database for AI, apps and agents", Lakebase subhead, CTAs.
3. https://www.databricks.com/product/lakebase — headline, subhead, body (verbatim anchors).
4. https://www.databricks.com/product/unity-catalog — headline, subhead, body (verbatim anchor).
5. https://www.databricks.com/product/genie — Genie One headline/subhead (register only).
6. https://www.databricks.com/company/newsroom/press-releases/databricks-acquires-row-zero-bringing-live-governed-spreadsheets — dateline, exec quote (verbatim anchor).
7. https://www.databricks.com/company/newsroom/press-releases/toyota-adopts-databricks-power-its-unified-data-and-ai-platform — press release structure, customer quote.
8. https://www.databricks.com/blog — recent titles (register only).
9. https://www.databricks.com/blog/how-choose-your-first-genie-agents-maximum-impact — opening line (verbatim anchor; only the second sentence's tail was returned verbatim).
10. https://www.databricks.com/company/careers — "innovators, builders and truthseekers" culture register.
11. https://www.databricks.com/customers — "Innovative companies lead with AI" (stories did not render).
12. https://www.linkedin.com/company/databricks/ — tagline and About text.
13. WebSearch "Databricks announces press release 2026" — press release titles/URLs.

Could NOT access:
- https://www.databricks.com/company/newsroom and /press-releases listings (no item text returned).
- https://www.youtube.com/@Databricks/about (consent redirect, not defeated).
- https://x.com/databricks (HTTP 402).
- Individual customer stories (page rendered "Loading...").
- LinkedIn/X post streams; no Apify spend.

Caveat: the summarizer paraphrased some sentence boundaries; the blog anchor is
kept to the short fragment returned as a direct quote.

## Social pass (2026-10-06, Apify)

# Databricks social sources

- Handles: X `@databricks` (twitter.com/databricks, from the databricks.com footer; author.userName verified as `databricks` in all items); LinkedIn `https://www.linkedin.com/company/databricks/` (author universalName `databricks`).
- X actor: apidojo/tweet-scraper, run tqTaK6GUeXPMBmYrP, dataset aTfeGQCFF1oGfK406. Input: twitterHandles [databricks], maxItems 40, sort Latest. Fetched 40; used 27 (13 retweets excluded; 0 replies).
- LinkedIn actor: harvestapi/linkedin-company-posts, run kk9CpciAUhSAaVxi7, dataset cBia5Zh7nd3QBZLCz. Input: targetUrls [company page], maxPosts 30. Fetched 30; used 29 (1 repost of an employee post excluded, not quoted).
- Approx cost: well under $0.05 total (about 14 s and 7 s runs, 40 + 30 items). Exact charge not read back.
- Lessons: no wrong slug, no block, no retry needed. The call-actor response reported 20 X items while the run was still finishing; the dataset held 40 on fetch. Raw files were written from the full dataset via the Apify API.
- Raw: raw-x.json, raw-linkedin.json (original posts only, {date,url,text}).
