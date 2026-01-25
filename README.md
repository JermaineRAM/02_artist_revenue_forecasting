# 📈 Artist Revenue Forecasting Under Uncertainty
## Project Overview

This project explores how historical streaming data can be used to estimate future royalty revenue for a music artist, with a focus on uncertainty, volatility, and realistic planning rather than precise prediction.

Rather than applying complex forecasting models by default, the analysis compares simple, interpretable approaches to assess which methods are most appropriate given the underlying data patterns. The project mirrors real-world scenarios where artists, managers, or labels need defensible revenue expectations rather than exact forecasts.

## Key Questions

The analysis was guided by the following questions:

 1. What does historical monthly royalty revenue look like for an individual artist?

 2. Is the revenue pattern stable, trending, or highly volatile?

 3. How do different simple forecasting approaches compare under volatile conditions?

 4. Which forecasting method provides the most practical and defensible estimate for planning?

## Dataset

The dataset is simulated to reflect realistic music streaming and royalty reporting structures and includes:

 - Monthly streaming usage across platforms and territories

 - Royalty rates applied per stream

 - Artist-level aggregation of expected revenue

A simulated dataset was used to allow full control over volatility, noise, and reporting behaviour while avoiding proprietary or sensitive financial data.

## Methodology

The analysis follows a structured, decision-focused workflow:

 1. Revenue construction

     - Combined streaming usage with royalty rates

     - Cleaned invalid stream values

     - Calculated expected revenue at the record level

 2. Time series aggregation

     - Aggregated revenue to monthly totals

     - Created a continuous time series suitable for forecasting

 3. Pattern inspection

     - Visualised historical revenue to assess volatility and trend

     - Identified spiky, irregular behaviour rather than smooth growth

 4. Forecast comparison

     - Compared three simple approaches:

         - Naive (last observed value)

         - Rolling average

         - Linear trend

 5. Forecast interpretation

     - Assessed realism and robustness rather than statistical accuracy

Visualisations were used to support interpretation and decision-making rather than to optimise predictive performance.

## Key Findings
### 1️⃣ Revenue Is Highly Volatile

Historical monthly revenue for the selected artist exhibits significant spikes and drops, with no clear long-term upward or downward trend.

This volatility is typical of real-world streaming income, where playlist placement, releases, and reporting cycles can cause abrupt changes.

### 2️⃣ Naive Forecasts Are Overly Reactive

Naive forecasts closely track the most recent observation, making them highly sensitive to short-term spikes or dips.

While simple, this approach risks overestimating or underestimating future income when recent months are atypical.

### 3️⃣ Trend Models Are Unstable in Noisy Data

Linear trend models attempt to impose structure on a dataset that does not exhibit a clear trend.

In this context, trend-based forecasts are highly sensitive to noise and may imply growth or decline that is not supported by the underlying pattern.

### 4️⃣ Rolling Averages Provide the Most Defensible Estimate

Rolling average forecasts smooth short-term volatility while remaining grounded in recent performance.

For spiky, trendless revenue data, this approach provides the most realistic and interpretable estimate for budgeting and planning purposes.

## Interpretation

The analysis demonstrates that model choice should be driven by data behaviour, not model sophistication.

In the absence of a clear trend, simpler smoothing-based approaches outperform more complex or assumption-heavy methods in terms of practical usefulness. For artists with volatile income streams, stability and transparency are more valuable than precision.

## Limitations
 - The dataset is simulated and does not represent actual artist earnings
 - External drivers (marketing, releases, playlists) are not modelled

 - No formal forecast accuracy metrics are calculated

The analysis prioritises decision relevance over predictive optimisation.

## Skills Demonstrated

 - Feature engineering and revenue construction

 - Time series aggregation and visualisation

 - Forecast comparison under uncertainty

 - Analytical judgement in model selection

 - Clear communication of limitations and trade-offs

## Conclusion

This project shows how simple, well-reasoned forecasting approaches can provide useful financial guidance in environments characterised by volatility and uncertainty.

By focusing on interpretability and realism rather than complexity, the analysis mirrors how forecasting is often applied in real-world music industry and business contexts.