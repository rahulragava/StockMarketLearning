## 📌 XIRR — Extended Internal Rate of Return

> “What is my effective annual return considering I invested and withdrew money at different times?”

### 🔍 Definition  
XIRR calculates the **annualized return** of an investment when **cash flows (inflows/outflows) occur at irregular dates**.  
It adjusts for both:
- **Amount** of each cash flow  
- **Exact date** it happened  

---

### 📊 When to Use  
- **Lump sum investments:** ✅ Works, same as CAGR  
- **SIP (Systematic Investment Plans):** ✅ Best choice  
- **Multiple additions/withdrawals:** ✅ Handles them perfectly  
- **Irregular deposits:** ✅ Corrects for timing differences  

---

### 📐 Formula (conceptual)  
$$
\sum_{i=1}^{n} \frac{C_i}{(1+R)^{\frac{\text{days}_i - \text{days}_0}{365}}} = 0
$$  
Where:  
- ( C_i ) = Cash flow (negative for investments, positive for withdrawals/final value)  
- \( R \) = XIRR (annualized return)  
- \( text{days}_i ) = Date of transaction  
- \( text{days}_0 ) = Date of first transaction  

---

### 📅 Example

| Date       | Amount    | Note |
|------------|-----------|------|
| 01-Jan-2021| -₹1,00,000| Initial investment |
| 01-Jul-2021| -₹50,000  | Additional investment |
| 01-Jan-2022| ₹20,000   | Partial withdrawal |
| 01-Jan-2023| ₹1,00,000 | Partial withdrawal |
| 01-Jan-2024| ₹80,000   | Final withdrawal |

- **Minus sign (–)** = money you invest (cash outflow)  
- **Plus sign (+)** = money you receive (cash inflow)  

---

### 📊 How to Calculate in Excel / Google Sheets  
Formula:
```
= XIRR(values, dates)
```
Example:
```
= XIRR(B2:B6, A2:A6)
```
Where:
- `values` = range of cash flow amounts (with correct signs)  
- `dates` = range of corresponding dates  

---

### 🆚 XIRR vs CAGR

| Feature                | CAGR | XIRR |
|------------------------|------|------|
| Handles multiple cash flows | ❌ | ✅ |
| Requires exact dates   | ❌ | ✅ |
| Ideal for SIP          | ❌ | ✅ |
| Ideal for lump sum     | ✅ | ✅ |

---

💡 **Tip:**  
If your mutual fund app or brokerage shows “CAGR” for a SIP, it might not reflect the *true* return — use XIRR for accuracy.

---

## Related Concepts
[[CAGR (Compound Annual Growth Rate)]]  
[[SIP (Systematic Investment Plan)]]
