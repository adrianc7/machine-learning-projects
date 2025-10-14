# World Happiness Analysis (2015–2019)

This project analyzes global happiness trends from 2015 to 2019 using data from the World Happiness Report, combining both R statistical analysis and an interactive Tableau dashboard to visualize findings across countries and regions.

---

## Project Overview
The goal of this analysis was to explore the factors influencing happiness worldwide, compare regions and countries, and identify key contributors such as GDP, health, social support, and freedom.  
The workflow integrates two major analytical approaches:
1. **R Analysis** – Data cleaning, correlation analysis, regression modeling, and statistical insights  
2. **Tableau Visualization** – Interactive storytelling and dashboarding for comparative and regional exploration

---

## Access the Tableau Dashboard
Explore the full interactive version here:  
[View on Tableau Public](https://public.tableau.com/app/profile/adrianchavezloya/viz/WorldHappinessAnalysis_17604612913100/Dashboard)

---

## Dataset Information

| Attribute | Description |
|------------|-------------|
| **Source** | World Happiness Report (via Kaggle & Gallup World Poll data) |
| **Years** | 2015–2019 |
| **Main Variables** | Country, Region, Happiness Score, GDP per Capita, Health (Life Expectancy), Social Support, Freedom, Generosity, Corruption |
| **Key Files Used** | `cleaned_world_happiness_2015_2019.csv`, `tableau_cleaned_world_happiness.csv`, `tableau_country_summary.csv`, `tableau_factor_importance_2019.csv` |
| **Data Purpose** | Evaluate global well-being and the relationship between economic, social, and health indicators with happiness |

---

## Repository Structure

| File | Description |
|------|--------------|
| `cleaned_world_happiness_2015_2019.csv` | Cleaned dataset used for R and Tableau analysis |
| `tableau_cleaned_world_happiness.csv` | Data formatted for Tableau import |
| `tableau_country_summary.csv` | Aggregated country-level data |
| `tableau_factor_importance_2019.csv` | Factor regression output for visualization |
| `happiness-analysis-using-r.ipynb` | R Notebook containing the statistical analysis and data processing |
| `happiness-analysis-using-r.pdf` | PDF export of the R notebook with outputs and plots |
| `World Happiness Analysis.twbx` | Packaged Tableau workbook |
| `World Happiness Analysis.pptx` | Summary presentation of key visuals |
| `README.md` | Project documentation |

---

## Analysis Process

### R Analysis
The analysis in R involved:
- Cleaning and combining data from multiple years (2015–2019)
- Calculating year-to-year rank and score changes
- Performing correlation analysis to identify key factors linked to happiness
- Building a multiple regression model to estimate variable importance
- Generating summary statistics and visualizations (boxplots, heatmaps, trends)

**R Key Findings**
- GDP, Health, and Social Support had the strongest positive correlations with Happiness (~0.78–0.79)  
- Freedom showed a moderate positive relationship (0.57)  
- Generosity and Perception of Corruption were relatively weaker predictors  
- Regression analysis showed that freedom and social support were statistically the most influential when combined with GDP and health

### Tableau Visualization
The Tableau dashboard visualizes happiness trends interactively, allowing users to explore by region, country, and score changes.  
Main components include:
- **Regional Comparison:** Displays average happiness by global region  
- **World Happiness Map:** Geographical heatmap of average scores  
- **Change by Rank (2015–2019):** Shows improvement or decline in rankings  
- **Countries by Avg. Score:** Highlights top-ranked nations  
- **Factor Importance (2019):** Visualizes variable impact (Freedom, Social Support, Health, etc.) derived from R regression results

---

## Comparison: R vs Tableau Results

| Aspect | R Statistical Analysis | Tableau Dashboard Visualization |
|--------|------------------------|----------------------------------|
| **Top Predictors** | GDP, Health, Social Support | Freedom, Social Support, Health |
| **Weakest Predictor** | Generosity | Generosity |
| **Global Pattern** | Europe & Oceania consistently happiest | Same confirmed visually through map and bar rankings |
| **Key Correlation Strengths** | Quantified precisely (r ≈ 0.78–0.84 for top factors) | Visualized relatively through bar magnitude and color shading |
| **Insights Presentation** | Numeric and inferential | Visual, exploratory, and comparative |

Both analyses confirm that wealth, health, and community support are the core pillars of happiness.  
R provided statistical rigor and quantification, while Tableau translated these insights into clear global visuals for public understanding.

---

## Key Insights
- **Freedom and Social Support** emerge as the most consistent contributors to happiness across all models, suggesting that psychological well-being and community connections matter more than pure economic factors once basic needs are met
- **Africa remains the least happy region** on average, while **Europe and Oceania consistently top rankings** - this likely reflects the stability of social institutions, healthcare access, and economic security in developed regions versus infrastructure challenges in many African nations
- **Venezuela showed the greatest improvement** in happiness rankings between 2015–2019, which is surprising given its economic collapse but may reflect resilience, strong social networks, or cultural adaptations during crisis
- **Zambia demonstrated significant improvement**, likely due to economic growth and infrastructure investments during this timeframe
- **Happiness inequality across regions has remained relatively stable**, though Western and Northern Europe continue to dominate, with Nordic countries consistently ranking highest due to their strong social safety nets, work-life balance, and high trust in institutions
- **The relationship between GDP and Happiness shows diminishing returns** after a threshold, implying non-economic factors increasingly matter in richer nations where basic needs are universally met
- **In Tableau's Factor Importance visualization, GDP appeared less significant** because it overlaps heavily with health and social support—both of which capture quality-of-life dimensions that go beyond pure income
- **This multicollinearity causes GDP's apparent influence to drop** when the combined model emphasizes well-being indicators rather than just economic scale
- **Many countries showed rank declines** potentially due to increasing political polarization, economic uncertainties, and the early impacts of climate-related stresses affecting life satisfaction globally

---

## License
This project uses publicly available data from the World Happiness Report (Gallup World Poll / Sustainable Development Solutions Network).  
Created for educational and analytical purposes to explore global well-being patterns.