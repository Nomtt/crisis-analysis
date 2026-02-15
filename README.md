# financial-crisis-visualization

This repository contains simple quantitative analysis of the 2008 Global Financial Crisis, focusing on the mechanical breakdowns in market confidence. By correlating the collapse of distressed institutions (**AIG, Citigroup**) with systemic stress indicators (**TED Spread, VIX**), this project models how liquidity crises mutate into solvency crises.

The analysis contrasts the "Risk Transfer" mechanism of 2008 (where public backstops absorbed losses) against the "survivor" metrics of resilient banks like JPMorgan.

---

### Financial & Economic implications

Beyond standard EDA, our project visualizes three critical economic phenomena:

#### 1. The "Risk Transfer" Mechanism (Private Loss to Public Liability)
The analysis quantifies the massive wealth destruction in the private sector that necessitated government intervention.
* **The Wipeout:** Equity holders in **AIG** and **Citigroup** saw near-total losses of **-99.5%** and **-98.0%** respectively.
* **The Implications:** Unlike a standard recession, this "fat tail" event shifted liability from private balance sheets to the public sector (via TARP). The code visualizes this by contrasting the total collapse of these firms against the **S&P 500's** relatively "mild" **-57%** drawdown, isolating the systemic risk premium.

#### 2. The "Psychological Cliff" (Breaking the Buck)
The notebook correlates the timing of the **Reserve Primary Fund** falling below $1.00 NAV (to $0.97) with the seizure of interbank lending.
* **Economic Intuition:** In money markets, a 3% loss is not just a dip—it is a contract failure. This small deviation triggered a non-linear panic response, proving that "safe" assets rely on binary trust (1.00 or bust) rather than fundamental valuation.

#### 3. Liquidity vs. Solvency (The Contagion Vector)
By overlaying the **TED Spread** (difference between 3-Month LIBOR and T-Bills) on equity prices, the analysis identifies the exact moment the crisis shifted from "Credit Concern" to "Liquidity Freeze."
* **Implication:** AIG didn't fail solely because of poor insurance underwriting; it failed because the interbank lending market (visualized by the TED spike) froze, denying them the short-term liquidity needed to post collateral.

---

### 🚀 Key Technical Features

* **Automated Data Pipeline:** Scripts to unzip and inventory complex financial datasets (`gfc.zip`) containing equities and macro indicators.
* **Multi-Institution Comparison:**
    * **Distressed Assets:** Tracks the collapse of **AIG** and **Citigroup** to model systemic failure.
    * **Control Group:** Contrasts these with **JPMorgan** (-68.1%) to isolate specific credit risk from general market beta.
* **Systemic Risk Modeling:**
    * **Credit Freeze:** Correlates equity collapses with spikes in the **TED Rate** and **VIX**.
    * **Volatility Clustering:** Maps the exact windows where market fear decoupled from fundamental asset prices.

---

### Analysis Summary

The notebook reconstructs the timeline of the 2008 crash through three analytical lenses:
1.  **Risk Transfer:** Visualizing the destruction of private equity value (AIG/Citi) vs. the resilience of survivors (JPM).
2.  **Market Stress:** Using the **VIX** to identify the transition from "correction" to "panic."
3.  **Interbank Trust:** Using the **TED Spread** as a proxy to identify when banks stopped trusting each other, preceding the broader equity market crash.

---

### Technologies Stack: 
Python, pandas, matplotlib
