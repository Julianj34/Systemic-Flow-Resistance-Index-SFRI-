# 📊 Systemic Flow Resistance Index (SFRI)

**A novel financial indicator for analyzing capital flow stability and systemic market friction — inspired by fluid dynamics.**

---

## 🚀 What is SFRI?

The **Systemic Flow Resistance Index (SFRI)** quantifies **how efficiently or inefficiently capital flows through a market**, similar to how liquids behave under pressure and resistance in fluid mechanics.

---

## 🧠 Concept & Analogy

| Financial Market     | Fluid Dynamics Equivalent |
|----------------------|---------------------------|
| Price Movement       | Pressure Difference       |
| Trading Volume       | Flow Rate                 |
| Spread (High - Low)  | Flow Resistance           |
| SFRI                 | Systemic Viscosity Index  |

- **High SFRI** = Capital congestion → potential volatility or stress buildup  
- **Low SFRI** = Smooth capital flow → structurally healthy markets

---

## 🧮 Formula

```python
Price Change = df['Close'].diff()
Effective Flow = df['Volume'] * abs(Price Change)
Spread = df['High'] - df['Low']
SFRI = (abs(Price Change) * Spread) / (Effective Flow + epsilon)
SFRI *= 10000  # For better readability
