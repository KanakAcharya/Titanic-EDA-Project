# Titanic Dataset - Exploratory Data Analysis (EDA)

## Overview

This project demonstrates a comprehensive **Exploratory Data Analysis (EDA)** on the Titanic dataset, showcasing essential data science skills including data cleaning, pattern discovery, statistical analysis, and professional visualization techniques.

**Dataset**: 891 passenger records with 15 features  
**Focus**: Data quality assessment, survival pattern analysis, and storytelling through visualizations

---

## Project Highlights

### ✅ Key Findings

**Survival Insights:**
- **Overall Survival Rate**: 38.4% (342 out of 891 passengers survived)
- **Gender Impact**: Women had significantly higher survival rates compared to men ("Women and children first" policy observed)
- **Class Impact**: First-class passengers had substantially better survival chances
- **Age Pattern**: Children had higher survival rates

**Data Quality Issues Identified:**
- Cabin deck: 688 missing records (77.2%)
- Age: 177 missing records (19.9%)  
- Embarkation: 2 missing records (0.2%)

---

## Dataset Information

| Attribute | Details |
|-----------|----------|
| **Records** | 891 passengers |
| **Features** | 15 columns |
| **File Format** | CSV (from Seaborn) |
| **Data Types** | Mixed (int, float, object, bool) |
| **Time Period** | April 1912 (RMS Titanic disaster) |

---

## Analysis Sections

### 1. **Data Loading & Initial Exploration**
- Dataset shape and structure
- Column information and data types
- First few rows examination
- Basic descriptive statistics (mean, median, std, min, max)

### 2. **Data Quality Assessment**
- Missing value identification and quantification
- Visual representation of missing data patterns
- Missing data impact analysis
- Data completeness evaluation

### 3. **Survival Analysis**
- Overall survival rate calculation
- Survival rate by gender (showing gender bias)
- Survival rate by passenger class
- Age distribution analysis
- Cross-tabular analysis for pattern identification

### 4. **Visualizations**
- Bar charts for categorical comparisons
- Histograms for distribution analysis
- Multiple subplots for comprehensive views
- Color-coded visualizations for clarity

---

## Technologies & Libraries

| Technology | Purpose |
|-----------|----------|
| **Python 3** | Programming language |
| **Pandas** | Data manipulation and analysis |
| **NumPy** | Numerical computations |
| **Matplotlib** | Static data visualization |
| **Seaborn** | Statistical visualization |
| **Jupyter Notebook** | Interactive analysis environment |

---

## How to Use This Project

### View on GitHub
1. Open the repository at: https://github.com/KanakAcharya/Titanic-EDA-Project
2. Click on the `.ipynb` file to view the notebook with all outputs rendered
3. GitHub automatically displays visualizations and formatted output

### Run Locally

**Prerequisites:**
```bash
pip install pandas numpy matplotlib seaborn jupyter
```

**Steps:**
```bash
# Navigate to project directory
cd Titanic-EDA-Project

# Launch Jupyter Notebook
jupyter notebook

# Open the notebook file in the browser
# Execute cells to see analysis and visualizations
```

---

## Skills Demonstrated

✅ **Data Exploration**
- Systematic dataset examination
- Identifying data structure and types
- Recognizing patterns and anomalies

✅ **Data Cleaning**
- Missing value detection and assessment
- Data quality evaluation
- Handling inconsistencies

✅ **Statistical Analysis**
- Descriptive statistics
- Aggregations and groupby operations
- Comparative analysis

✅ **Data Visualization**
- Chart selection based on data type
- Color-coded visualizations
- Multi-plot layouts
- Proper labeling and formatting

✅ **Problem-Solving**
- Pattern identification
- Hypothesis formation
- Insight generation

✅ **Communication**
- Clear documentation
- Structured analysis
- Professional presentation

---

## Key Code Features

### Data Loading
```python
import seaborn as sns
df = sns.load_dataset('titanic')
```

### Missing Value Analysis
```python
missing = df.isnull().sum()
missing_percent = (missing / len(df)) * 100
```

### Survival Aggregation
```python
df.groupby('sex')['survived'].agg(['sum', 'count', 'mean'])
df.groupby('pclass')['survived'].mean()
```

### Professional Visualizations
```python
plt.subplots(2, 2, figsize=(14, 10))
sns.set_style('whitegrid')
```

---

## What Recruiters Value

This EDA project demonstrates to potential employers:

✓ **Practical Data Skills** - Real-world analysis techniques
✓ **Problem-Solving** - Pattern discovery and insight generation  
✓ **Code Quality** - Clean, well-documented, reproducible code
✓ **Visualization Skills** - Effective communication through charts
✓ **Attention to Detail** - Handling data quality issues systematically
✓ **Business Acumen** - Drawing actionable insights from data

---

## Project Structure

```
Titanic-EDA-Project/
├── README.md                          # Project documentation
├── Titanic_EDA_Analysis.ipynb         # Main analysis notebook
└── requirements.txt                   # Python dependencies
```

---

## Future Enhancements

- 🔄 Feature engineering for predictive modeling
- 🔗 Correlation and heatmap analysis
- 🤖 Machine learning models (Logistic Regression, Random Forest)
- 📊 Advanced visualizations (violin plots, pair plots, heatmaps)
- 🧪 Hypothesis testing and statistical significance
- 📈 Time-based pattern analysis

---

## Key Insights & Learnings

1. **Data Quality Matters**: Missing data in Cabin (77%) requires handling decisions
2. **Visual Exploration First**: Charts reveal patterns that raw numbers might hide
3. **Categorical Analysis**: Gender and class are strong predictors of survival
4. **Documentation is Key**: Clear comments and section headers improve readability
5. **Storytelling with Data**: Presenting findings as a coherent narrative is crucial

---

## Author

**Kanak Acharya**  
Data Science Professional | Biology Educator | Competitive Exam Aspirant

---

## License

This project is open source and available under the **MIT License**.  
Feel free to use, modify, and distribute for educational purposes.

---

## Acknowledgments

- **Dataset Source**: Seaborn built-in datasets (originally from Kaggle)
- **Tools**: Python data science community (Pandas, Matplotlib, Seaborn)
- **Inspiration**: Real-world application of EDA best practices

---

## Questions & Support

If you have questions about this analysis:
- Review the notebook comments for detailed explanations
- Check inline documentation in code cells
- Refer to library documentation (Pandas, Matplotlib, Seaborn)

---

**Last Updated**: February 28, 2026  
**Status**: ✅ Complete and Production-Ready
