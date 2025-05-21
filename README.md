# How Frozen Job Market is overall per state
Yes, you can calculate how **“frozen”** the job market is in each state using these datasets by constructing a **Frozen Market Index** at the state level, similar to your national-level index. Here's how:

---

### 🧊 **Frozen Market Index by State** 
You can use a weighted or unweighted composite index that **adds signs of dysfunction** and **subtracts signs of tightness** in the labor market:

#### ✅ Add (↑ = More Freeze):

These indicate dysfunction, slack, or friction:

* **Unemployed persons per job opening**
* **Layoffs and discharges rate**
* **Total separations rate**

#### ❌ Subtract (↓ = More Freeze):

These indicate demand or strength:

* **Job openings rate**
* **Hires rate**
* **Quits rate** (voluntary quits = worker confidence)

---

### 🧮 Suggested Formula (Unweighted Example)

```text
Frozen_Market_Index_state = 
(+ z(Unemployed per Job Opening)) 
+ z(Layoffs Rate)
+ z(Separations Rate)
- z(Job Openings Rate)
- z(Hires Rate)
- z(Quits Rate)
```

You can normalize each variable using **z-scores** (by state over time or across all states) to make them comparable before averaging or summing them.

---

### ✅ Required Data from Your Chart List

You can pull these values from the chart dropdown:

* ✅ `State job openings rates map`
* ✅ `State hires rates map`
* ✅ `State total separations rates map`
* ✅ `State quits rates map`
* ✅ `State layoffs and discharges rates map`
* ✅ `State unemployed persons per job opening map`

---

### 📊 What You'll Get

For each state and time period (e.g., monthly), you'll produce a **Frozen Market Index score**, where:

* **Higher = more frozen**
* **Lower = more fluid/healthy**

You can visualize it as:

* Choropleth maps (darker = more frozen)
* Time-series lines (each state = one line)
* Heatmaps (states vs months)

---

If you'd like, I can help you:

* Build the formula in Python or SQL
* Guide the Tableau chart design
* Normalize and weight the indicators

Would you like to proceed with implementation using one of your data sources?
