# 02_artist_revenue_forecasting
Artist revenue forecasting using historical streaming data to produce clear, explainable royalty income projections.

This project focuses on forecasting an artist’s future royalty income using historical streaming data.

Rather than relying on complex or black-box machine learning models, the analysis prioritises **clear, interpretable forecasting methods** that reflect how revenue projections are commonly used in the music industry. The goal is to produce forecasts that artists, managers, or label teams could realistically understand and apply when planning releases, tours, or budgets.

The project builds a clean monthly revenue time series from streaming data and explores multiple forecasting approaches, including baseline, rolling average, and trend-based projections. Emphasis is placed on transparency, assumptions, and limitations, mirroring real-world decision-support analytics rather than purely academic modelling.

**Note:** The dataset used in this project is simulated but designed to reflect real-world music royalty reporting structures, including volatility, platform differences, and reporting noise.

This analysis is framed from the perspective of an artist or management team seeking realistic expectations around future income rather than precise financial guarantees.

---

## Project Objective

The goal of this project is to answer a practical business question:

**“Based on past streaming performance, what can an artist reasonably expect to earn over the next few months?”**

Rather than attempting to produce a single ‘perfect’ prediction, the project compares multiple simple forecasting approaches to understand how different assumptions affect revenue expectations.

---

## Data Overview

The analysis uses a simulated dataset representing:
- Streaming usage across **100 fictional artists**
- Multiple platforms and territories
- Monthly reporting over multiple years

For forecasting, the analysis focuses on a **single artist (Phoenix Santos)**, while retaining the wider catalogue to provide realistic context.

---

## Methodology

### 1. Revenue Time Series Construction

Reported streaming usage for the selected artist is combined with royalty rate data to calculate **expected monthly revenue**. Negative stream values are clipped to zero to avoid unrealistic revenue calculations.

Revenue is then aggregated to a monthly time series, forming the foundation for all forecasting methods.

---

### 2. Catalogue Context

Before forecasting, the artist’s total streams are compared against the wider catalogue to understand their relative position. This mirrors real-world workflows where forecasts are interpreted differently for head, mid-tier, or long-tail artists.

---

### 3. Forecasting Approaches

Three simple and interpretable forecasting methods are applied:

#### Naive Baseline  
Assumes the next period will match the most recent observed month.  
This method serves as a benchmark but is highly sensitive to short-term volatility.

#### Rolling Average  
Uses a short rolling window to smooth month-to-month fluctuations.  
This approach provides a more stable estimate and is often preferred for budgeting and planning.

#### Trend Projection  
Fits a simple linear trend to historical data and projects it forward.  
With volatile data, this method can overreact to noise and is therefore treated cautiously.

Forecasts are only shown **after the final observed data point**, reflecting real-world uncertainty rather than retroactively fitting history.

---

## Key Findings and Interpretation

Phoenix Santos’ monthly revenue exhibits **significant volatility** with no strong long-term upward or downward trend.

- The **naive forecast** reacts strongly to the most recent month and can be misleading when revenue spikes or dips.
- The **trend-based forecast** shows limited reliability due to the absence of a clear directional pattern.
- The **rolling average forecast** provides the most reasonable planning estimate, as it smooths volatility without assuming sustained growth or decline.

This comparison highlights the importance of matching forecasting methods to data behaviour rather than defaulting to more complex models.

---

## Limitations and Assumptions

- The dataset is simulated and does not represent actual royalty statements.
- Forecasts do not account for future releases, marketing campaigns, or external shocks.
- Results are intended to support **planning and expectation-setting**, not precise financial forecasting.

---

## Conclusion

This project demonstrates how simple, transparent forecasting methods can provide meaningful insights when applied thoughtfully. In cases of volatile artist revenue, stable approaches such as rolling averages often outperform more reactive or assumption-heavy models.

The analysis emphasises **interpretability, realism, and judgement**, mirroring how forecasting is used in real music industry and data-driven decision-making contexts.