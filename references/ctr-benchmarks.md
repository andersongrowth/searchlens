# CTR Benchmarks — SearchLens

## Standard CTR by Position (Desktop, Non-Branded, No SERP Features)

These are widely referenced industry averages. Use as baseline — actual values vary by niche, query type, and SERP layout.

| Position | CTR Benchmark | Notes |
|---|---|---|
| 1 | 28–35% | Wide range depending on brand recognition |
| 2 | 13–15% | Significant drop from position 1 |
| 3 | 9–11% | |
| 4 | 6–8% | |
| 5 | 5–7% | |
| 6 | 4–6% | |
| 7 | 3–5% | |
| 8 | 3–4% | |
| 9 | 2.5–3.5% | |
| 10 | 2–3% | Bottom of page 1 — still meaningful |
| 11–15 | 0.8–1.5% | Page 2 — very low organic value |
| 16–20 | 0.3–0.8% | |
| 21–30 | 0.1–0.3% | Near-invisible |

**CTR gap threshold for flagging:** If actual CTR is more than 2 percentage points below the benchmark for that position, flag as underperforming.

---

## CTR Adjustments by Query Type

These are multipliers/adjustments to apply on top of the standard benchmarks.

### Branded Queries
- Position 1 branded CTR: 50–70% (users are looking for you specifically)
- Position 2–3 branded: 15–25%
- **Implication:** Always segment branded from non-branded before CTR analysis. Mixing inflates apparent CTR performance.

### Informational Queries ("how to", "what is", "guide")
- Standard benchmarks apply
- Featured snippet present → position 1 CTR drops to 8–15% (snippet captures clicks)
- "People Also Ask" boxes reduce CTR for positions 2–5 by approximately 20–30%

### Navigational Queries (brand + product name)
- Similar to branded: position 1 CTR 45–65%
- Less useful for optimization — users already have intent locked in

### Commercial Queries ("best X", "top X", "X review", "X vs Y")
- Position 1: 20–28% (slightly lower than informational — users comparison-shop)
- Shopping ads above organic results reduce all organic CTR by 15–25%

### Transactional Queries ("buy X", "X price", "X near me")
- Organic CTR significantly lower due to ads
- Position 1 organic with ads present: 10–18%
- Position 1 organic without ads: 25–35%
- Local pack present (3-pack): reduces organic CTR below the fold by 30–40%

### Question Queries (who, what, when, where, why, how)
- Featured snippet captured: position 0 CTR = 8–12%, position 1 CTR drops to 5–10%
- No snippet: standard benchmarks apply

---

## CTR by Device Type

| Position | Desktop CTR | Mobile CTR |
|---|---|---|
| 1 | 32% | 26% |
| 2 | 14% | 11% |
| 3 | 10% | 8% |
| 4–7 | 5–7% | 4–6% |
| 8–10 | 2.5–4% | 2–3% |

**Key insight:** Mobile CTR is consistently 15–25% lower than desktop for the same position. If your site is mobile-heavy, use the mobile column as the benchmark.

---

## CTR Impact of SERP Features

These features appear between position 1 and the rest of organic results, depressing CTR for everyone below:

| SERP Feature | CTR Impact on Organic |
|---|---|
| Featured Snippet (position 0) | Reduces pos 1–3 CTR by 20–30% |
| Knowledge Panel | Reduces CTR across all positions by 10–20% |
| Local Pack (3-pack) | Reduces below-pack organic CTR by 30–40% |
| Shopping Ads (4+ ads) | Reduces all organic CTR by 20–35% |
| Image Pack | Minor impact (~5–10% reduction) |
| Video Carousel | Reduces positions 1–5 CTR by 10–20% |
| People Also Ask (4+ boxes) | Reduces positions 2–5 CTR by 15–25% |

**Practical application:** When CTR is lower than benchmark but the page ranks well, check for SERP features before concluding the title is the problem.

---

## CTR Improvement Benchmarks (After Optimization)

When a title/meta is rewritten with best practices, typical CTR gains:

| Starting CTR vs Benchmark | Expected Recovery |
|---|---|
| 50%+ below benchmark | 40–70% of the gap can be recovered |
| 25–50% below benchmark | 30–50% recovery |
| Under 25% below benchmark | 15–30% recovery — may be SERP feature issue |

**Formula for estimating clicks gained from CTR optimization:**
```
Current clicks = Impressions × Current_CTR
Target CTR = Current_CTR + (CTR_gap × recovery_rate)
Estimated new clicks = Impressions × Target_CTR
Clicks gained = Estimated_new_clicks - Current_clicks
```

---

## Title Best Practices for CTR Improvement

When recommending a title rewrite, apply these rules:

**Must have:**
- Primary keyword in the first 40 characters
- Specific number or year when applicable ("7 estratégias" or "Guia 2025")
- Clear value proposition or outcome

**Avoid:**
- Generic openers ("Tudo sobre...", "Saiba mais sobre...")
- Titles longer than 60 characters (truncated in SERP)
- Keyword stuffing (more than 2 uses of the same keyword)
- Passive or vague language ("Como pode ser feito X")

**High-CTR title formulas:**
1. `[Number] + [Adjective] + [Keyword] + [Benefit]`
   → "7 Estratégias de Link Building que Funcionam em 2025"
2. `Como [Keyword] + [Specific Outcome]`
   → "Como Fazer Auditoria de SEO Técnico em 60 Minutos"
3. `[Keyword]: [Specific Promise]`
   → "SEO On-Page: O Checklist Completo (Atualizado 2025)"
4. `[Question format for featured snippet targeting]`
   → "O Que é PageRank e Como Ele Funciona em 2025?"
