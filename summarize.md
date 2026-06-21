# Shopee: Strengthening Customer Intelligence and Marketing Optimisation
**Course:** MRTB2123 Business Analytics — Case Study 1
**Programme:** MSc Business Intelligence & Analytics (AI), Universiti Teknologi Malaysia
**Supervisor:** Assoc. Prof Ts Dr Nur Azaliah bt Abu Bakar
**Team:** Umar Syukri (MRT254044) · Soo Wai San (MRT254005) · Nur Aisyah Binti Ahmad Zaki (MRT254043) · Rosmaili Binti Ibrahim (MRT254015) · Erwan Fadly Bin Sudiman (MRT254011)

---

## Executive Summary

Shopee's GMV is growing, but margins are declining. The root cause is not a marketing budget problem — it is an **analytics maturity problem**. Four structural gaps (data fragmentation, descriptive-only analytics, weak segmentation, and poor recommendations) form a compounding feedback loop that keeps Shopee at the descriptive stage of the Analytics Maturity Model, leaving it analytically immature relative to AI-native competitors like TikTok Shop and Lazada.

**Proposed solution:** A four-layer analytics framework (CDP → Descriptive → Predictive → Prescriptive) delivered via a phased hybrid strategy targeting a CLV:CAC ratio exceeding 3:1.

---

## Section 1 — Problem Understanding

**Business Context:**
- Dominant e-commerce platform across 7 SEA markets
- GMV and active users growing, but operating margins under persistent pressure
- Rising Customer Acquisition Cost (CAC) and escalating promotional expenditure
- AI-native competitors reshaping the competitive landscape

**Central Challenge:**
> How can Shopee design and implement an integrated business analytics strategy that transforms fragmented data into actionable intelligence, enabling precise customer targeting, effective personalisation, and sustainable marketing performance?

| Symptom | Systemic Cause |
|---|---|
| Declining retention, high churn | No churn prediction, weak segmentation |
| Rising CAC, declining ROMI | Descriptive-only analytics |
| Generic campaigns, low CTR | Fragmented customer profiles |
| Margin erosion from over-discounting | Cannot distinguish customer types |

---

## Section 2 — Analytical Diagnosis

Four structural limitations operating as a **compounding feedback loop**:

1. **Data Fragmentation** — Customer data distributed across disconnected systems with no unified customer ID; prevents 360-degree profiling and degrades all downstream analytics.
2. **Descriptive Analytics Reliance** — Analytics anchored at "what happened" dashboards; no predictive churn models or CLV estimation; decisions are reactive, not proactive.
3. **Insufficient Behavioural Segmentation** — Segments defined only by GMV or login frequency; cannot distinguish promotion-dependent from brand-loyal customers.
4. **Weak Recommendation System** — Rule-based logic and historical data only; repetitive suggestions and limited discovery; forgoes the data network effect that TikTok Shop exploits.

**The Vicious Cycle:** Data fragmentation degrades segmentation → poor segmentation produces unreliable predictive outputs → organisation reverts to descriptive-only reporting → weak recommendations starve the analytical layers of useful signal.

---

## Section 3 — Analytics Application Framework

A four-layer architecture designed to invert the compounding feedback loop from vicious to virtuous:

### L1 — Foundation: Unified Customer Data Platform (CDP)
- Consolidates transactional records, browsing behaviour, campaign interactions, demographic profiles, and seller signals
- Single persistent customer ID enabling a 360-degree customer view
- Real-time segmentation and activation capability
- **Prerequisite for all layers above it**

### L2 — Descriptive: Behavioural Metric Dashboards
Restructured from aggregate GMV to individual-level signals:
- Browse-to-purchase ratio
- Category dwell time
- Discount-redemption rate
- Session recency and frequency
- Cart-abandonment frequency

### L3 — Predictive: Three Techniques

| Technique | Method | Key Outputs |
|---|---|---|
| Behavioural Segmentation | K-Means / Extended RFM | Promotion-dependent, brand-loyal, convenience, high-intent segments |
| Churn Prediction | XGBoost / LightGBM | Declining session frequency, cart abandonment, reduced campaign engagement |
| CLV Estimation | BG/NBD + Gamma-Gamma | Expected purchase frequency, monetary value per purchase, per-segment budgeting |

### L4 — Prescriptive: Highest Value Layer

**Hybrid Recommendation Engine:**
- Collaborative filtering (similar user profiles)
- Content-based filtering (category/attribute match)
- Real-time signals (current browsing session)
- Serendipity injection (prevents filter bubble formation)

**Next-Best-Action Optimisation:**

| Segment | Signal | Action |
|---|---|---|
| Promotion-Dependent Customer | High churn risk, moderate CLV | Targeted time-limited voucher |
| Brand-Loyal Customer | Low churn risk, high CLV | No discount (margin preserved) |
| High-Intent Browser | Pre-conversion, high CLV potential | Personalised recommendation |

---

## Section 4 — Strategic Evaluation

### 4.1 Strategic Pairs Comparison

| Strategy | Scalability | Cost-Effectiveness | Ethical Risk | Competitive Position |
|---|---|---|---|---|
| Mass Marketing | High | Low | Low | Weak |
| Personalised Marketing | High (ML) | High | Moderate | Strong |
| Rule-Based Systems | Low | Moderate | Low | Weak |
| AI-Driven Systems | Very High | High | High | Essential |
| Promotion-Led Acquisition | High | Low | Low | Declining |
| CLV-Led Retention | High (ML) | High | Moderate | Sustainable |

### 4.2 Cross-Cutting Ethical Implications
- **Data Privacy & PDPA** — Explicit consent and data minimisation across all 7 SEA markets
- **Algorithmic Bias & Fairness** — Systematic auditing across merchant categories, languages, and demographics
- **Filter Bubble Prevention** — Diversity-aware algorithms as standard design requirement
- **User Autonomy** — Personalisation Transparency Dashboard for user control and opt-out
- **AI Explainability** — Human-readable explanations for decisions affecting seller visibility

### 4.3 Recommended: Phased Hybrid Strategy

| Phase | Timeline | Priority Actions | Target KPI |
|---|---|---|---|
| P1 — Foundation | Months 1–6 | CDP implementation, improved rule-based segmentation, mass marketing retained for 11.11/12.12 | Data Quality Score |
| P2 — Personalisation | Months 6–18 | ML personalisation, CLV modelling, hybrid rule-based + AI architecture, PDPA compliance | CLV:CAC > 2:1 |
| P3 — Responsible AI | Months 18–36 | Explainability modules, quarterly bias auditing, serendipity injection, Transparency Dashboard | CLV:CAC > 3:1 |

---

## Section 5 — Solution Design and Implementation

| Component | Implementation | Expected Outcome |
|---|---|---|
| Unified CDP | Integrate all data sources under a single customer ID | Complete customer view, accurate attribution, real-time activation |
| Behavioural Segmentation | K-Means on purchase intent, loyalty, and churn risk | Better targeting, reduced wasted promotional spend |
| Churn Prediction Model | XGBoost trained on behavioural signals | Earlier retention interventions, improved profitability |
| CLV Estimation Model | BG/NBD + Gamma-Gamma per customer and segment | Budget allocated proportional to projected long-term value |
| AI Recommendation Engine | Hybrid collaborative + content-based + real-time | Improved product discovery, higher engagement, larger basket size |
| AI Governance | Consent controls, quarterly bias audits, explainability | Lower compliance risk, stronger consumer trust across SEA |

### Expected Business Impact
- **> 3:1** CLV:CAC ratio (Phase 3 target)
- **2–5x** conversion rate improvement via personalisation
- **35%** of revenue attributable to personalised recommendations
- Churn reduced through earlier predictive interventions
- Elimination of over-discounting to brand-loyal customers
- Competitive gap with TikTok Shop narrowed via data network effect

---

## Conclusion

> *"The competitive advantage is not data. It is decision quality."*

1. Shopee's challenge is an **analytics-maturity problem**, not a marketing-budget problem — symptom-level interventions are self-defeating.
2. The four-layer framework **inverts the compounding feedback loop** from vicious to virtuous.
3. The phased hybrid strategy aligns analytical capability with business strategy at every stage.
4. Responsible AI governance is a **competitive differentiator**, not a compliance cost.
