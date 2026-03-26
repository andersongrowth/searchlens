# searchlens

**A Claude Code skill that analyzes Google Search data and turns it into prioritized SEO actions.**

---

## About

SearchLens takes raw search data — Google Search Console exports, keyword research CSVs, ranking reports — and transforms it into clear, structured, actionable insights.

It doesn't just describe the data. It diagnoses what's wrong, explains why it matters, and tells you exactly what to do next.

---

## What it analyzes

| Input | Typical columns |
|---|---|
| GSC Performance Export | Query, Page, Clicks, Impressions, CTR, Position |
| Keyword Research CSV | Keyword, Volume, KD, CPC, Intent |
| Ranking Report | URL, Keyword, Position, Date |
| Content Gap File | Competitor URLs vs your URLs |
| Crawl Export | URL, Status, Title, H1, Words |

---

## What it produces

Every analysis runs through a structured pipeline:

1. **Data Health Check** — date range validation, anomaly flags, sample size warnings
2. **Quick Wins** — striking distance keywords (pos 8–20), CTR underperformers, cannibalization signals
3. **Content Gap Analysis** — topics competitors rank for that you don't
4. **Trend Signals** — rising and declining pages, volatility detection
5. **Intent Mapping** — classifies keywords by informational / commercial / transactional intent and flags format mismatches
6. **Priority Action List** — numbered, ordered by expected impact, with specific URLs and recommendations

---

## Files

```
searchlens/
├── SKILL.md                          # Core analysis logic and output format
└── references/
    ├── ctr-benchmarks.md             # CTR by position, device, and SERP feature
    ├── algorithm-updates.md          # Google update history for drop correlation
    └── intent-patterns.md            # Keyword intent classification patterns
```

---

## Installation

1. Download `searchlens.skill`
2. In Claude.ai, go to **Settings → Skills**
3. Click **Install skill** and upload the file

---

## Usage

Just drop a CSV or paste your data into the conversation. SearchLens triggers automatically when you share Google Search data and want analysis.

**Example prompts:**
- *"Here's my GSC export from the last 90 days — what should I focus on?"*
- *"I have this keyword list, help me prioritize it"*
- *"My traffic dropped in March, can you figure out why?"*
- *"Run a cannibalization audit on this ranking report"*

---

## Output format

```
## SearchLens Report
Data: [what was analyzed, date range, record count]
Data health: [flags or limitations]

### 🔍 Key Findings
### 📈 Quick Wins
### 🧱 Content Opportunities
### ⚠️ Issues to Fix
### 📊 Trends
### ✅ Priority Actions
```

---

## Built by

Made for [blader/humanizer](https://github.com/blader/humanizer) — a Claude Code skill that removes signs of AI-generated writing from text.
