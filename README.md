# World Happiness Report 2024 Analysis (PYTHON)

## Table of Contents
- [Overview](#overview)
- [Questions to Answer](#questions-to-answer)
- [Tools and Technologies](#tools-and-technologies)
- [Data Preparation and Exploratory Data Analysis (EDA)](#data-preparation-and-exploratory-data-analysis-eda)
  - [Data Loading and Cleaning](#data-loading-and-cleaning)
  - [Descriptive Statistics and Visualizations](#descriptive-statistics-and-visualizations)
  - [Correlation Analysis](#correlation-analysis)
- [Key Findings and Insights](#key-findings-and-insights)
  - [Happiest Countries](#happiest-countries)
  - [Geographical Trends](#geographical-trends)
  - [Evolution of Happiness Over Time](#evolution-of-happiness-over-time)
  - [Changes in Happiness by Country](#changes-in-happiness-by-country)
  - [Impact of Economic and Social Factors](#impact-of-economic-and-social-factors)
  - [Relationships with GDP, Corruption, and Freedom](#relationships-with-gdp-corruption-and-freedom)
- [Conclusions](#conclusions)
- [How to Run the Project](#how-to-run-the-project)

## Overview

This project analyzes the World Happiness Report 2024 dataset to derive meaningful insights about happiness across different countries. The dataset includes various indicators such as GDP per capita, social support, healthy life expectancy, perceptions of corruption, and freedom to make life choices. The primary goal is to understand global happiness trends and identify the key factors that contribute to higher or lower levels of happiness.

## Questions to Answer

1. Which countries are the happiest and why?
2. Are there geographical trends in happiness?
3. How has happiness evolved globally over the years?
4. Which countries have seen the greatest changes in happiness over time?
5. Which factors have the most significant impact on happiness?
6. What is the relationship between GDP and happiness?
7. How do perceptions of corruption correlate with happiness?
8. How do freedom to make life choices and happiness relate?

## Tools and Technologies

- **Python:** Primary programming language.
- **Pandas & NumPy:** Data manipulation and analysis.
- **GeoPandas:** Handling and visualizing geographic data.
- **Matplotlib & Seaborn:** Data visualization.
- **Jupyter Notebook:** Interactive analysis and documentation.
- **Data Source:** World Happiness Report (Kaggle dataset) and Natural Earth Data for geographical information.

## Data Preparation and Exploratory Data Analysis (EDA)

### Data Loading and Cleaning

- **Loading the Data:**  
  The dataset is imported using Pandas, and initial inspection reveals 2363 records with 11 columns.
  
- **Missing Data Check:**  
  Several columns (e.g., Log GDP per capita, Social support, Healthy life expectancy, etc.) contain missing values. Records with missing values were removed, resulting in a cleaned dataset of 2097 records.
  
- **Data Integrity:**  
  Duplicate rows were checked for and none were found, ensuring data uniqueness.

### Descriptive Statistics and Visualizations

- **Descriptive Statistics:**  
  Basic statistics such as mean, median, standard deviation, and range were computed for key variables (e.g., Life Ladder, Log GDP per capita, Social support).
  
- **Distribution Visualizations:**  
  Histograms with KDE overlays were plotted for the Life Ladder, Social support, and Log GDP per capita variables to assess their distributions and check for normality.

### Correlation Analysis

- **Correlation Matrix:**  
  A correlation heatmap was generated to identify relationships between variables such as Life Ladder, Log GDP per capita, Social support, and Healthy life expectancy. This step provided insight into which factors are most closely associated with happiness.

## Key Findings and Insights

### Happiest Countries

- **Top 10 Happiest Countries:**  
  Countries such as Finland, Denmark, Iceland, Switzerland, and Norway rank highest in happiness. High Life Ladder scores in these countries correlate with strong economic performance, robust social support systems, and high life expectancy.

### Geographical Trends

- **Regional Differences:**  
  Northern Europe consistently shows high levels of happiness, whereas Africa and parts of Asia exhibit lower scores. Developed regions, including North America and Australia, also generally report higher happiness levels compared to developing regions.

### Evolution of Happiness Over Time

- **Temporal Trends:**  
  The analysis of median Life Ladder scores over the years reveals fluctuations with a significant drop around 2006, gradual recovery through 2007–2019, and a steady rise from 2020 to 2023, indicating global improvements in well-being.

### Changes in Happiness by Country

- **Greatest Increases and Decreases:**  
  Countries such as Nicaragua, Bulgaria, and Serbia have experienced significant increases in happiness over time, while others like Pakistan, Zambia, and Afghanistan have seen notable declines, highlighting regional and political impacts on well-being.

### Impact of Economic and Social Factors

- **Key Influencers:**  
  - **Log GDP per Capita:** Shows the strongest positive correlation with happiness (≈ 0.79), indicating that economic prosperity plays a major role.
  - **Social Support and Healthy Life Expectancy:** Both are strongly correlated with happiness, emphasizing the importance of community support and healthcare.
  - **Perceptions of Corruption:** A moderate negative correlation (≈ -0.45) suggests that lower corruption levels contribute to higher happiness.

### Relationships with GDP, Corruption, and Freedom

- **GDP and Happiness:**  
  A scatter plot analysis shows a clear positive relationship between GDP per capita and Life Ladder scores.
  
- **Corruption and Happiness:**  
  Increased perceptions of corruption correlate with lower happiness scores.
  
- **Freedom and Happiness:**  
  A positive correlation (≈ 0.53) exists between the freedom to make life choices and happiness, though it is not as strong as economic factors.

## Conclusions

The World Happiness Report 2024 analysis indicates that happiness is a multifaceted phenomenon influenced by economic stability, social support, good healthcare, low corruption, and personal freedom. The findings suggest that policies aimed at boosting economic growth, enhancing social support networks, improving healthcare, and reducing corruption could collectively enhance national well-being.

## How to Run the Project

1. **Clone the Repository:**
```
git clone <URL_REPOZYTORIUM>
```

2 **Install Dependencies**:
Ensure you have Python 3.x installed. Then, install the required libraries:
```
pip install -r requirements.txt
```

3. Run the Jupyter Notebook: Launch the notebook server:
```
jupyter notebook
```

Open the file ```World Happiness Report 2024.ipynb``` and run the cells in sequence.

