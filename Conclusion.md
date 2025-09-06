# Video Game Sales – Simple Summary

**Goal:** Learn from past data (up to 2016) to help plan for **2017**.

**Data window used:** **2013–2016** (last 4 years with enough data).  
*Note: 2016 may be incomplete.*  
Sales numbers are in **USD millions**.

---

## What I did
- Cleaned the data (lowercase columns, fixed types, handled “TBD” as missing).
- Kept review scores as they are (no guessing).
- Created **global_sales = NA + EU + JP + Other**.

---

## Key findings

### Releases over time
- Peak year earlier was **2008** (~**1,427** games).
- Recent counts: **2013: 544**, **2014: 581**, **2015: 606**, **2016: 502**.

### Platforms (2013–2016)
- Top by global sales: **PS4, PS3, XOne, 3DS, X360, WiiU**.
- Typical platform life cycle ≈ **7 years**.
- For the same game released on many platforms:
  - **PS4** had the **most wins** (highest sales for that game) — **232** titles.
  - Average share across multi-platform games: **PS4 ~33.8%**, **PS3 ~20.8%**, **XOne ~11.8%**.

### Genres (share of global sales)
- **Action (29.5%)**, **Shooter (21.4%)**, **Sports (13.8%)** lead the market.

### Regions (top platform share)
- **North America:** PS4 **24.8%**, XOne **21.3%**, X360 **18.7%**  
- **Europe:** PS4 **36.0%**, PS3 **17.3%**, XOne **13.2%**  
- **Japan:** 3DS **48.2%**, PS3 **16.6%**, PSV **13.2%**

### Ratings (share of sales)
- **NA:** **M (37.7%)**, **E (18.1%)**, **Unknown (20.4%)**  
- **EU:** **M (37.0%)**, **E (21.3%)**, **Unknown (20.1%)**  
- **JP:** **Unknown (60.4%)**, **T (14.6%)**, **E (10.8%)**  
*(Japan uses CERO; many ratings show as “Unknown” in this dataset.)*

### Reviews and sales (PS4)
- **Critic score vs sales:** **r = 0.407** (moderate positive, **N=252**)
- **User score vs sales:** **r = −0.032** (near zero, **N=257**)
- Sales are **hit-driven** (a few blockbusters). Look at medians, not only totals.

---

## Hypothesis tests (user ratings, α = 0.05)

1. **Xbox One vs PC**  
   - *p* = **0.1476**; 95% CI = **[−0.090, 0.593]**; Cohen’s *d* = **0.162**  
   - **Result:** No clear difference in average ratings.

2. **Action vs Sports**  
   - *p* = **1.45e-20**; 95% CI = **[1.291, 1.907]**; Cohen’s *d* = **1.083**  
   - **Result:** **Action** games have **higher** average ratings than **Sports** by a large margin.

---

## Recommendations for 2017
- **Platforms:** Focus **PS4** globally; keep **XOne** strong in **NA/EU**; include **3DS** for **JP**.
- **Genres:** Prioritize **Action** and **Shooter**; keep **Sports** as a steady third.
- **Reviews:** Aim for strong **critic** coverage (critic scores relate to sales more than user scores on PS4).
- **By region:** Match the top platforms and genres listed above for each region.

---

## Limits
- 2016 data may be incomplete; some ratings are missing or mapped.
- Sales distribution is uneven (few titles make most of the money).

