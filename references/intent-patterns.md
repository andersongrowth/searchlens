# Intent Patterns — SearchLens

## The Four Intent Types

Search intent determines what content format Google will rank for a query. Getting the format wrong creates a ranking ceiling that no amount of optimization can overcome.

---

## Informational Intent

**What the user wants:** Knowledge, explanation, how-to guidance, understanding of a topic.

**Keyword modifiers and signals:**

| Category | Examples |
|---|---|
| Question words | como, o que é, por que, quando, onde, quem, what, how, why, when |
| Learning signals | guia, tutorial, aprenda, entenda, explicação, dicas, passo a passo, overview |
| Definition signals | o que é, definição, significa, conceito, diferença entre |
| Example signals | exemplos de, como funciona, demonstração |
| Comparison (educational) | diferença entre X e Y, X vs Y (when both options are concepts, not products) |

**SERP signals confirming informational intent:**
- Featured snippets
- "People Also Ask" boxes
- Wikipedia or educational site in position 1–3
- Blog posts and guides dominating top results

**Recommended content format:**
- Long-form blog post or guide (1.500–4.000 words)
- Clear H2/H3 structure addressing subtopics
- FAQ section for PAA targeting
- Definitions, examples, step-by-step sections

**Common mismatch:** Ranking a product/service page for an informational query. Position ceiling: 8–15. Fix: create a dedicated informational page, link it to the product page.

---

## Navigational Intent

**What the user wants:** A specific website, page, or brand.

**Keyword signals:**
- Brand name alone: "Ahrefs", "Google Analytics"
- Brand + feature: "Semrush keyword explorer", "GSC search console"
- Brand + action: "Netflix login", "Spotify download"
- "[brand] + review/pricing" — borderline navigational/commercial

**SERP signals confirming navigational intent:**
- Sitelinks appear under position 1
- Brand's own site is position 1 (always, unless brand penalty)
- Wikipedia or Crunchbase in top 5

**Recommended content format:**
- Homepage or primary product page for your own brand
- If optimizing for someone else's brand: create comparison or review content (commercial intent strategy)

**Optimization value:** Low for third-party sites. Focus on branded terms only for your own brand — ensure your homepage/key pages are well-linked and technically clean.

---

## Commercial Investigation Intent

**What the user wants:** To evaluate options before deciding. Research phase, not yet buying.

**Keyword modifiers and signals:**

| Category | Examples |
|---|---|
| Superlatives | melhor, top, melhores, best, top 10, leading |
| Comparison | vs, versus, comparação, alternativas, alternatives, diferença |
| Evaluation | review, avaliação, vale a pena, is X worth it, pros e contras |
| Recommendations | recomendação, indicação, sugestão, recommend |
| Selection | como escolher, qual é melhor, how to choose |

**SERP signals confirming commercial intent:**
- Listicles ("10 melhores X") in positions 1–5
- Review sites (G2, Capterra, Trustpilot, TechTudo) in top results
- Comparison tables in featured content

**Recommended content format:**
- Comparison page: "X vs Y — qual é melhor em 2025?"
- Listicle: "Os 10 Melhores [Produto/Serviço] para [Use Case]"
- Review page: first-person evaluation with pros/cons, specific test results
- Must include: specific data points, side-by-side comparisons, clear winner recommendation

**Common mismatch:** Ranking a generic blog post for a "best X" query, or a product page for a comparison query. The post needs to feel like a curated recommendation, not a sales page.

---

## Transactional Intent

**What the user wants:** To complete an action — buy, sign up, download, hire, get a quote.

**Keyword modifiers and signals:**

| Category | Examples |
|---|---|
| Purchase signals | comprar, buy, order, purchase, adquirir |
| Price signals | preço, quanto custa, price, custo, valor, cotação |
| Action signals | download, baixar, instalar, assinar, contratar, hire, get |
| Free trial / demo | grátis, free, trial, demo, teste gratuito |
| Proximity (local) | perto de mim, near me, em [cidade], [neighborhood] |
| Urgency | hoje, agora, rápido, entrega imediata |

**SERP signals confirming transactional intent:**
- Google Ads (text ads) above organic
- Shopping ads (product listings with images and prices)
- Local pack (for local transactional)
- E-commerce sites in positions 1–5

**Recommended content format:**
- Product or service landing page
- Clear CTA above the fold
- Price, plan details, or "get started" flow visible without scrolling
- Trust signals: testimonials, logos, certifications
- No-friction conversion path

**Common mismatch:** Ranking a blog post or category page for a high-intent transactional query. These pages cannot convert and often lose to dedicated landing pages. Fix: create a dedicated landing page, use the blog post to funnel traffic to it.

---

## Mixed Intent Queries

Some queries have ambiguous or split intent. Google often shows a mixed SERP.

**Examples:**
- "email marketing" → mix of informational (what is it) + commercial (tools)
- "SEO" → informational + navigational (tools) + commercial (services)
- "link building" → informational guides + commercial agency listings

**Strategy for mixed intent:**
- Check the actual SERP: what content types appear in positions 1–5?
- If 60%+ is one intent type, optimize for that format
- If truly split: create two pages (one informational, one commercial) and cross-link them

---

## Intent Classification Quick Reference

Use these signals to classify a keyword list rapidly:

```
IF keyword contains: como, o que é, por que, guia, tutorial, passo a passo
  → Informational

IF keyword contains: melhor, top, review, vs, alternativa, comparação, vale a pena
  → Commercial

IF keyword contains: comprar, preço, contratar, download, grátis, perto de mim
  → Transactional

IF keyword is: [brand name] or [brand + feature/page]
  → Navigational

IF unclear: check the SERP — the content type in positions 1–3 reveals Google's intent interpretation
```

---

## Intent Mismatch Detection

For each keyword-URL pair in the dataset:

| Current page type | Query intent | Mismatch? | Ceiling |
|---|---|---|---|
| Blog post / guide | Informational | No | None |
| Blog post / guide | Transactional | Yes | Position 8–15 |
| Blog post / guide | Commercial | Partial — listicle format needed | Position 5–10 |
| Product/service page | Transactional | No | None |
| Product/service page | Informational | Yes | Position 10–20 |
| Product/service page | Commercial | Partial — needs comparison elements | Position 5–12 |
| Category page | Commercial | Depends on format | Variable |
| Homepage | Navigational (branded) | No | None |

**Reporting format for mismatches:**
```
Intent Mismatch Detected:
Query: "melhor ferramenta de SEO"
Intent: Commercial (SERP shows listicles and comparison pages)
Your ranking URL: /blog/ferramentas-de-seo (informational blog post)
Current position: 14
Ranking ceiling: ~position 8 maximum with this format
Fix: Create /melhores-ferramentas-de-seo as a dedicated comparison/listicle page
Estimated position potential after fix: 3–8 (based on domain authority and backlinks)
```
