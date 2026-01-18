# Website Performance Analysis: Grammy Awards Digital Platform Strategy

## Executive Summary

This project evaluates The Recording Academy's February 2022 strategic decision to split its digital presence into two specialized websites: **Grammy.com** (entertainment/events) and **RecordingAcademy.com** (professional resources). Through comprehensive engagement analytics, the analysis demonstrates that the platform split successfully serves distinct audience segments with optimized user experiences.

---

## 📊 View This Analysis

- **GitHub Repository:** [grammys-website-analysis](https://github.com/rasumeng/Grammys-Website-Analysis) - Full code and documentation
- **Interactive Kaggle Notebook:** [Website Performance Analytics: Grammy Awards Platform Split Strategy](https://www.kaggle.com/code/robertasumeng/website-performance-analytics-grammy-awards) - Explore visualizations and run cells interactively

---

## Key Findings

### 1. **Extreme Event-Driven Traffic Concentration**
- Grammy Awards Show Night generates **43x traffic spike** (1.39M visitors vs. 32K regular days)
- This concentration represents both opportunity (massive peak engagement) and challenge (minimal year-round traffic)
- The domain split directly addresses this by creating specialized platforms for event vs. professional audiences

### 2. **Engagement Quality: Recording Academy Outperforms**

| Metric | Combined Site (Pre-Split) | Grammy.com (Post-Split) | RecordingAcademy.com |
|--------|---------------------------|------------------------|----------------------|
| **Bounce Rate** | 40.16% | 41.58% | **33.67%** ✓ |
| **Avg Session Duration** | 82.99s | 102.85s (+24%) | **128.50s** (+55%) |
| **Interpretation** | Baseline | Event-optimized | Professional-optimized |

**Finding:** RecordingAcademy.com demonstrates superior engagement metrics, indicating that professional audiences find specialized industry-focused content significantly more relevant than mixed entertainment/professional content.

### 3. **Mobile-First Platform Usage**
- **68% mobile traffic** on Grammy.com (April-June 2023)
- Reflects real-time Grammy Awards viewing behavior (checking results on smartphones during broadcast)
- Requires mobile-first design optimization for both platforms

### 4. **Demographic Segmentation Success**
- Grammy.com attracts broad entertainment audiences across all age groups
- RecordingAcademy.com demonstrates higher engagement from music industry professionals and educators
- Platform separation successfully allows each site to serve its intended demographic

### 5. **Competitive Position**
Compared to American Music Awards (industry benchmark):
- Grammy.com **bounce rate 12.7pp lower** (41.58% vs. AMA's 54.31%) ✓ Superior engagement
- Session duration differs due to seasonal timing (Grammy data includes off-season periods)
- Mobile optimization is competitive advantage given 68% mobile traffic

---

## Strategic Recommendations

1. **Continue Two-Site Strategy** - Differentiated engagement metrics justify maintaining specialized platforms rather than combining audiences

2. **Enhance Grammy.com Year-Round Content** - Develop off-season content strategy to sustain engagement between awards while optimizing for mobile

3. **Expand RecordingAcademy.com Resources** - Strong engagement metrics (lowest bounce rate, longest sessions) indicate market demand for professional content; recommend continued investment

4. **Monitor Conversion Metrics** - Engagement doesn't guarantee business success; track conversions to memberships, tickets, and other revenue drivers

5. **Mobile Optimization Priority** - With 68% mobile traffic, ensure both platforms deliver fast load times and responsive design

---

## Project Structure

### Core Analysis
- **`grammys-analysis.ipynb`** - Complete analytical notebook with data exploration, visualizations, and findings

### Data Files  
- `grammy_live_web_analytics.csv` - Daily traffic before/after Feb 1, 2022 organizational split
- `ra_live_web_analytics.csv` - Recording Academy platform daily metrics
- `grammys_age_demographics.csv` - Age group distribution on Grammy.com
- `tra_age_demographics.csv` - Age group distribution on RecordingAcademy.com
- `desktop_users.csv` - Desktop traffic April-June 2023
- `mobile_users.csv` - Mobile traffic April-June 2023

---

## How to Run

### Prerequisites
```bash
pip install pandas plotly jupyter
```

### Launch Analysis
```bash
jupyter notebook
# Open: grammys-analysis.ipynb
```

All data files are automatically loaded from the `datasets/` folder.

---

## Methodology & Important Caveats

**Analysis Scope:**
- Engagement metrics only (bounce rate, session duration, pages per session)
- Traffic concentration and audience segmentation analysis
- Pre/post February 1, 2022 split comparison

**Important Limitations:**
- **Correlation ≠ Causation:** Changes observed post-split correlate with platform separation but may result from other factors (marketing, content improvements, technical enhancements)
- **Engagement ≠ Revenue:** Higher engagement doesn't guarantee business outcomes; conversion metrics are essential for complete evaluation
- **Seasonality:** Grammy Awards drives extreme seasonal variation; off-season patterns may not represent full platform potential

---

## Dataset Definitions

| Field | Definition |
|-------|-----------|
| **visitors** | Unique daily user visits |
| **pageviews** | Total pages viewed across all sessions |
| **sessions** | Number of distinct user sessions |
| **bounced_sessions** | Sessions where users left without interaction |
| **avg_session_duration_secs** | Average time per session in seconds |
| **awards_night** | Date of Grammy Awards ceremony |
| **bounce_rate** | (bounced_sessions ÷ total_sessions) × 100 |

---

## Contact & Attribution

**Analysis Date:** January 2026  
**Data Period:** Through June 2023  
**Portfolio Project:** Website Performance Analytics & Strategic Evaluation

---

## Key Insight

> The website split represents a successful strategic choice to serve distinct audiences with optimized experiences. Rather than forcing entertainment and professional audiences into a single platform, The Recording Academy created specialized sites that allow each audience to find relevant, engaging content aligned with their interests. The data supports continuing this approach while investing in specialized content for each platform's core audience.
