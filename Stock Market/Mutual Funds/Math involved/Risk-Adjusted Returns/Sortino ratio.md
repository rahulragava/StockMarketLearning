## 📌 Sortino Ratio #ReturnByRisk 

> "How much extra return am I getting for the *bad* risk I’m taking?" — Focuses only on downside risk, not all volatility.

---

### **🔍 Simple Meaning**

- The Sortino Ratio is like the Sharpe Ratio but **ignores upside volatility** (good swings).  
- It only considers **downside volatility** — the harmful drops in returns below a certain threshold (often the risk-free rate or 0%).  
- This makes it **more forgiving** to investments with high positive volatility (big upward movements).

---

### **📌 Why Use It?**
- #SharpeProblem  The Sharpe Ratio can penalize investments that are volatile *upwards*. 
- The Sortino Ratio focuses on **risk of loss** instead of total fluctuations.  


---

### **🎯 Example**
If a fund has:  
- Many big gains (high upside volatility)  
- A few small losses (low downside volatility)  
The Sharpe Ratio might undervalue it, but the Sortino Ratio will score it higher because it only measures risk from losses.

---

### **📌 Formula**
$$
Sortino\ Ratio = \frac{R_p - R_f}{\sigma_d}
$$

Where:  
- \( R_p \) = Portfolio return  
- \( R_f \) = Risk-free return  
- \( sigma_d ) = **Downside deviation** (standard deviation of returns below the target)

---


# Sortino Ratio — Simple Example

> "Sortino Ratio tells you how much return you get for the risk of losing money, ignoring the good swings."

---

## **Step 0 — What We Have**

- Monthly portfolio returns: `2%, -1%, 3%, -2%, 1%, 4%, 0%, -3%, 5%, 2%, -1%, 3%`  
- Risk-free rate per month = 0.33% (0.0033 in decimal)  

We'll calculate **Sortino Ratio** using **only months with negative performance** compared to risk-free rate.

---

## **Step 1 — Identify Bad Months**

A “bad month” = month where return < 0.33%  

|Month|Return (%)|Decimal|Compare to 0.33%|
|---|---|---|---|
|1|2|0.02|0.02 > 0.0033 → Good|
|2|-1|-0.01|-0.01 < 0.0033 → Bad|
|3|3|0.03|Good|
|4|-2|-0.02|Bad|
|5|1|0.01|0.01 > 0.0033 → Good|
|6|4|0.04|Good|
|7|0|0|0 < 0.0033 → Bad|
|8|-3|-0.03|Bad|
|9|5|0.05|Good|
|10|2|0.02|Good|
|11|-1|-0.01|Bad|
|12|3|0.03|Good|

**Bad months**: 2, 4, 7, 8, 11  

---

## **Step 2 — Convert to Decimal & Calculate Downside Differences**

- Risk-free per month = 0.33% → 0.0033  
- Bad months returns in decimal: -0.01, -0.02, 0, -0.03, -0.01  
- Difference from target (Rf):  

| Bad Month | Return | Difference from 0.0033 | Squared difference |
| --------- | ------ | ---------------------- | ------------------ |
| 2         | -0.01  | -0.0133                | 0.00017689         |
| 4         | -0.02  | -0.0233                | 0.00054289         |
| 7         | 0      | -0.0033                | 0.00001089         |
| 8         | -0.03  | -0.0333                | 0.00110889         |
| 11        | -0.01  | -0.0133                | 0.00017689         |

---

## **Step 3 — Calculate Downside Deviation**

1. Square the differences  
2. Average the squares  (≈0.00040329)
3. Take the square root  

$$
\sigma_d \approx 0.0152
$$

---

## **Step 4 — Average Portfolio Return**

- Monthly average return: 1.60% → 0.0160  
- Excess return over Rf:  

$$
\text{Excess Return} = 0.0160 - 0.0033 = 0.0127
$$

---

## **Step 5 — Calculate Sortino Ratio**

$$
\text{Sortino Ratio} = \frac{\text{Excess Return}}{\sigma_d}
$$

$$
\text{Sortino Ratio} = \frac{0.0127}{0.0152} \approx 0.835
$$

---

## ✅ **Step 6 — Interpretation**

- Sortino = 0.835 → Good risk-adjusted return considering **only the bad months**.  
- Higher value → Better returns per unit of **downside risk**.  

---

## Quote

> "Sortino focuses on the risk you actually fear — losing money — and ignores the swings that make you richer."

---

## Related Concepts
[[Sharpe Ratio]]  
[[Volatility]]  
[[Standard Deviation]]
