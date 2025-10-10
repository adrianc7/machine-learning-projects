# Key Indicators of Life Expectancy in Developing Countries

This project analyzes health and economic data from the World Health Organization (WHO) and the United Nations to understand which factors most strongly affect life expectancy in developing countries.  
The data covers 193 countries from 2000 to 2015 and includes health, education, and income indicators.

---

## Overview

- **Dataset:** `Life Expectancy Data.csv` (193 countries, 2000–2015)  
- **Goal:** Identify which social, health, and economic factors have the greatest influence on life expectancy.  
- **Methods Used:**  
  - Simple Linear Regression  
  - Quadratic Regression  
  - Multiple Linear Regression  
  - Variance Inflation Factor (VIF) analysis to check for overlapping effects between variables  

---

## What Was Done

1. **Explored the Relationship Between GDP and Life Expectancy**  
   - Found that wealthier countries tend to have longer life expectancy, but the effect slows down after a certain point (a curved, not straight-line relationship).

2. **Built Models Using Multiple Factors**  
   - Added variables such as adult mortality, infant deaths, education, vaccination rates, BMI, income distribution, and HIV/AIDS rates.  
   - These models explained over **82%** of the differences in life expectancy between countries.

3. **Removed Redundant Variables**  
   - GDP and health expenditure were removed because they were too closely related to other variables.  
   - This improved the reliability of the final model.

---

## Key Findings

- **Adult Mortality, Infant Deaths, and HIV/AIDS** → Lower life expectancy  
- **Education (Schooling)** → Higher life expectancy  
- **Income Composition of Resources** → Higher life expectancy  
- **Vaccination Rates (Diphtheria, Polio)** → Higher life expectancy  
- **BMI (Healthy Weight Levels)** → Higher life expectancy  
- **Alcohol Consumption** → Lower life expectancy  
- **GDP** → Related to life expectancy, but its effect overlaps with other social and health factors

The final model explained about **82%** of the variation in life expectancy across developing countries, meaning these key variables provide a strong picture of what drives population health.

---

## Interpretation

Countries with:
- Lower adult and infant mortality  
- Higher education levels  
- Broader vaccination coverage  
- Stronger income equality  
- Lower HIV/AIDS rates  

tend to have citizens who live significantly longer, healthier lives.  
**This highlights that life expectancy is influenced not just by a country’s wealth, but by access to healthcare, education, and equitable social conditions**.

---

## Repository Contents

| File | Description |
|------|-------------|
| `key_indicators_life_expectancy.ipynb` | Python notebook with all analysis and models |
| `key_indicators_life_expectancy.pdf` | Exported version of the notebook with results and visuals |
| `Life Expectancy Data.csv` | WHO/UN dataset used for analysis |

---

## Conclusion

**Improving life expectancy in developing countries depends on more than just raising GDP — it requires investing in education, public health, and disease prevention**.  
