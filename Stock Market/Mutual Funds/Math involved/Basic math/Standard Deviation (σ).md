> "How jumpy the returns are" — a measure of how much an investment’s returns move up or down from the average.

Standard deviation is a statistical measure that tells you how spread out the values in a dataset are around the mean (average). It gives you an idea of the typical distance between each data point and the mean.

---

## What is Standard Deviation?

- **Low standard deviation** means data points are close to the average — consistent results.
- **High standard deviation** means data points are spread out — more variability.
- It is expressed in the same units as the data.
- Used to measure risk or volatility in investments, like mutual funds and stocks.

---

## How to Calculate Standard Deviation (Step-by-Step)

Imagine monthly returns (%) of a mutual fund for 5 months:

| Month | Return (%) |
|-------|------------|
| 1     | 8          |
| 2     | 12         |
| 3     | 10         |
| 4     | 11         |
| 5     | 9          |

---

### Step 1: Calculate the Mean (Average) Return

$$
\text{Mean} = \frac{8 + 12 + 10 + 11 + 9}{5} = \frac{50}{5} = 10\%
$$

---

### Step 2: Calculate Deviations from Mean

| Month | Return (%) | Deviation from Mean = Return – Mean |
|-------|------------|-------------------------------------|
| 1     | 8          | 8 - 10 = -2                        |
| 2     | 12         | 12 - 10 = 2                       |
| 3     | 10         | 10 - 10 = 0                       |
| 4     | 11         | 11 - 10 = 1                       |
| 5     | 9          | 9 - 10 = -1                       |

---

### Step 3: Square Each Deviation

| Month | Deviation from Mean | Squared Deviation (²) |
|-------|---------------------|----------------------|
| 1     | -2                  | 4                    |
| 2     | 2                   | 4                    |
| 3     | 0                   | 0                    |
| 4     | 1                   | 1                    |
| 5     | -1                  | 1                    |

---

### Step 4: Calculate Variance (Average of Squared Deviations)

$$
\text{Variance} = \frac{4 + 4 + 0 + 1 + 1}{5 - 1} = \frac{10}{4} = 2.5
$$

---

### Step 5: Calculate Standard Deviation (Square Root of Variance)

$$
\text{Standard Deviation} = \sqrt{2.5} \approx 1.58\%
$$

---

## What Does This Mean?

- The returns typically vary by ±1.58% around the average return of 10%.
- Lower standard deviation means less risky and more consistent returns.
- Higher standard deviation means more ups and downs — greater risk.

---

## Standard Deviation in [[Sharpe Ratio]]

The Sharpe Ratio measures how much return you get for the risk taken and uses standard deviation as the risk measure:

$$
\text{Sharpe Ratio} = \frac{\text{Return of Investment} - \text{Risk-free Return}}{\text{Standard Deviation of Investment Returns}}
$$

- **Standard deviation here is the measure of investment's risk or volatility.**
- A **higher Sharpe ratio** means better returns per unit of risk.
- A **lower Sharpe ratio** indicates either lower return or higher risk.

---

# Summary

- Standard deviation = how much your data (returns) vary from the average.
- Used widely in finance to understand investment risk.
- Calculated by finding the mean, deviations, squaring, averaging (variance), and square-rooting.

---

