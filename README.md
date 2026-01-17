# Time-Series-Sales-Forecasting-and-Demand-Planning
# Overview
This project demonstrates how time-series forecasting can be used to support inventory planning, marketing decisions, and seasonal demand management for a consumer goods business.

Using R and statistical modeling, I forecasted sales for a highly seasonal ice-cream product (“Wisp”) by combining:

- Marketing impact analysis

- Trend and seasonality modeling

- ARIMA-based forecasting

Due to data confidentiality, raw datasets and full code cannot be shared. This case study focuses on approach, insights, and business relevance.

# Business Problem

Seasonal consumer products face recurring challenges:

- Strong demand peaks and troughs

- Risk of overstocking outside peak seasons

- Difficulty linking marketing spend to sales outcomes

- Limited visibility into short-term future demand

Key questions addressed:

- How can next-month sales be forecasted reliably?

- How strong is seasonality, and how should inventory respond?

- Which marketing activities meaningfully impact sales?

- How can forecasts guide inventory and promotion planning?

# Solution Approach

I designed a two-layer forecasting framework combining marketing effectiveness analysis with time-series modeling.

**🔹 Marketing Impact Analysis**

- Built a multiple linear regression model to quantify the effect of:

- Advertising channels

- Promotions

- Applied logarithmic transformation to stabilize variance

- Validated model assumptions using diagnostic plots

**🔹 Time-Series Forecasting**

- Analyzed regional sales patterns independently

- Tested stationarity using ADF tests

- Applied differencing to handle trend and seasonality

- Built ARIMA models for each region

- Validated forecasts using an 80:20 train–test split

- Evaluated accuracy using MAPE

**🔹 Forecast Output**

- Generated region-level sales forecasts for the upcoming month

- Delivered demand signals suitable for inventory and planning decisions

# Key Business Insights & Impact

- Clear seasonality detected, with strong sales peaks during warmer months
 → Inventory planning must be tightly aligned with seasonal forecasts

- Marketing effectiveness varied by channel
 → TV advertising delivered stronger ROI than banners or promotions

- Urban and high-density regions drove most demand
 → Regional forecasting improves allocation of stock and marketing spend

- Forecasts enabled proactive planning
 → Reduced risk of stock-outs during peak demand and excess inventory off-season

# Strategic Recommendations

- Use time-series forecasts as a baseline for inventory planning

- Align production and replenishment with seasonal demand curves

- Allocate marketing budgets toward channels with proven sales impact

- Refresh forecasts monthly to adapt to changing demand conditions

- Treat regional demand separately instead of using global averages

# Tools & Technologies

- R

- Time-Series Modeling: ARIMA

- Statistical Analysis: Multiple Linear Regression

- Forecast Evaluation: MAPE

- Visualization: ggplot2

# Why this Matters for Your Business

This project shows how time-series forecasting can:

- Improve inventory accuracy for seasonal products

- Reduce waste and lost sales

- Support smarter marketing investment decisions

- Turn historical sales data into forward-looking planning tools

The same approach applies to:

- Seasonal retail products

- FMCG and consumer goods

- Weather-sensitive demand categories

- Short-term demand planning problems

# 📌 Confidentiality Note

This project was completed using a confidential academic dataset.

Raw data and full code cannot be shared publicly.

# 💬 How I Can Help You

If your business needs to:

- Forecast seasonal sales

- Improve inventory and replenishment planning

- Understand demand cycles and peaks

I can adapt this framework to your real sales data and deliver:

- Time-series forecasts

- Demand insights

- Planning-ready outputs

- Clear business recommendations
