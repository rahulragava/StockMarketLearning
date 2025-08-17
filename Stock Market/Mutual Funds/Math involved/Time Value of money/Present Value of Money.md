## 📌 Present Value (PV) — Time Value of Money

> “How much is a future amount of money worth today, given a specific interest rate or required return?”

---

### 🔍 Definition  
**Present Value (PV)** is the current worth of a sum of money to be received in the future, discounted at a specific rate of return.  
It reflects the principle that **money now is more valuable than money later** due to its earning potential.

---

### 💡 Opportunity Cost Connection  
The discount rate used in PV calculation is often your **opportunity cost** — the return you could earn by investing the money elsewhere.  
- If inflation and alternative investment returns are high, future cash flows are worth less today.  
- PV helps you decide if an investment’s future returns justify the cost today.

---

### 📐 Formula (Annual Compounding)  
$$
PV = \frac{FV}{(1 + r)^n}
$$

Where:  
- **FV** = Future value (amount to be received in the future)  
- **r** = Annual discount rate / required return (decimal form)  
- **n** = Number of years

---

### 📅 Example — Using Opportunity Cost  
You expect to receive ₹1,50,000 in 5 years, and your opportunity cost (discount rate) is 8% per year.  

1. \( 1 + r = 1.08 \)  
2. Raise to the power of n: \( 1.08^5 \approx 1.4693 \)  
3. Divide FV by this: \( ₹1,50,000 \div 1.4693 \approx ₹1,02,062 \)  

So ₹1,50,000 in 5 years is worth **₹1,02,062 today** if your required return is 8%.

---

### 📊 Example — Investment Decision  
If you can buy an asset for ₹1,00,000 today and expect to sell it for ₹1,50,000 in 5 years:  

- **Required return** = 8% → PV ≈ ₹1,02,062 → Worth buying (since PV > cost)  
- **Required return** = 12% → PV ≈ ₹85,226 → Not worth buying (since PV < cost)

---

### 🔄 Relation to CAGR & FV  
- **PV** works backward: Given **FV**, **r**, **n** → find today’s worth.  
- **FV** works forward: Given **P**, **r**, **n** → find future worth.  
- **CAGR** finds the rate: Given **P**, **FV**, **n** → find **r**.

Formulas:  

$$
FV = P \times (1 + r)^n
$$  

$$
PV = \frac{FV}{(1 + r)^n}
$$  

$$
r = \left( \frac{FV}{P} \right)^{\frac{1}{n}} - 1
$$

---

## Related Concepts
[[Future Value of money]]  
[[CAGR (Compound Annual Growth Rate)]]  
[[XIRR (Extended Internal Rate of Return)]]  
