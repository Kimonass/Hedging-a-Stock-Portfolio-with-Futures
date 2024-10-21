
## 1. Executive Summary
The primary objective of this report is to demonstrate how risk can be effectively reduced in a well-structured and diversified portfolio through the use of futures contracts. Additionally, the report outlines the development of an automated process that can be applied to any portfolio and index.
Metrics Comparison:

Key findings regarding the portfolio’s performance are as follows:
- **Standard Portfolio:**
  - Mean Return: **0.0785**
  - Standard Deviation: **0.9690**
  - Sharpe Ratio: **0.0810**
  - Max Drawdown: **0.1234**
  - Value at Risk: **-1.6933**
  
- **Hedged Portfolio:**
  - Mean Return: **0.0779**
  - Standard Deviation: **0.9165**
  - Sharpe Ratio: **0.0850**
  - Max Drawdown: **0.1201**
  - Value at Risk: **-1.4453**

These results indicate that while both portfolios exhibit similar performance characteristics, the hedged portfolio demonstrates a lower standard deviation and a higher Sharpe ratio, suggesting improved risk-adjusted returns.

The observation, through a process of trial and error, is that in a poorly performing portfolio (unlike the current well-diversified one), risk can be reduced by up to 40% with the current hedging strategy. While this insight isn’t explicitly included in the recommendations, it is a noteworthy observation based on prior experience.

---

## 2. Introduction
The goal of this analysis is to assess the effectiveness of using futures contracts as a hedging strategy to mitigate risk in a well diversified portfolio. This analysis seeks to test if the systematic hedging can enhance the overall risk-return profile of an investment portfolio.

The scope of this report covers a holding period from **October 8, 2023, to September 8, 2024**, utilizing data collected from **Yahoo Finance** for general market data and **Investing.com** specifically for FTSE ATHEX Large Cap data.

---

## 3. Data Collection and Methodology
Data was collected from reliable financial sources including **Yahoo Finance** for general stock prices and **Investing.com** for specific indices.

### Normalization
Normalization of the values was performed primarily for visualization and comparative purposes, allowing for a clear graphical representation of performance trends across the different portfolios.

### Assumptions
Several assumptions were made during the analysis:
- The portfolio is taken from a previous project, ensuring continuity in the investment strategy.
- The hedge ratio is recalculated every three days.
- A margin requirement of **10%** is established.
- The value of the hedged portfolio is derived from the portfolio value adjusted by the profit and loss (P&L) flow.
- Beta calculations are based on a rolling window of **45 days**.
- The formula used for calculating the number of contracts is:

$$
\text{Number of contracts} = -\beta \times \left( \frac{\text{portfolio value}}{\text{index price} \times \text{multiplier}} \right)
$$


Where the change in price is modeled as:



$$
ΔS = a + \beta \cdot ΔF + \epsilon
$$

And

$$
\beta = \text{hedge ratio} = ρ \left( \frac{σ_s}{σ_F} \right)
$$

---

## 6. Performance Analysis
Visualizations included in this report effectively illustrate the comparative performance of the standard and hedged portfolios.

### Key Performance Metrics
The key metrics that have been utilized in this analysis include:
- Standard Deviation
- Sharpe Ratio

---

## 7. Conclusion
The analysis demonstrates that employing futures contracts as a hedging mechanism effectively reduces the risk profile of a well-performing portfolio. Key findings from the analysis reveal:
- The hedged portfolio exhibited a lower standard deviation (0.00917) and a higher Sharpe ratio (0.08496) than the standard portfolio, suggesting a favorable adjustment in risk-return characteristics.
- The hedging strategy can provide significant benefits, especially in scenarios where the portfolio might underperform.

### Recommendations
Moving forward, it is recommended to maintain the current hedging strategy while continuously monitoring market conditions. In cases of anticipated poor performance, further enhancements to the hedging process may be necessary to ensure robust risk management.

