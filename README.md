# FIFA World Cup 2026 Predictions

**Hex Hackathon Submission** - Data-driven predictions and insights for the 2026 FIFA World Cup

## Project Overview

This project analyzes 150+ years of international soccer data to predict outcomes for the 2026 FIFA World Cup - the first tournament with an expanded 48-team format. Using machine learning models and interactive visualizations, we uncover patterns in team performance, historical trends, and generate predictions for potential matchups.

## Datasets

- **results.csv**: 48,891 international match results (1872-2025)
- **goalscorers.csv**: 44,447 individual goal records
- **shootouts.csv**: 662 penalty shootout outcomes
- **former_names.csv**: Country name changes over time

## Methodology

### 1. Data Analysis
- Historical trend analysis of World Cup matches
- Team performance metrics (win rate, goals scored, goal difference)
- Recent form analysis (2022-2025) for current team strength

### 2. Feature Engineering
- Win rate calculations
- Goals per match averages
- Goal difference metrics
- Neutral venue adjustments
- Tournament-specific patterns

### 3. Machine Learning Models
- **Logistic Regression**: Baseline classification model
- **Random Forest**: Ensemble learning for robust predictions
- **Gradient Boosting**: Advanced boosting for accuracy

Trained on major tournament matches (FIFA World Cup, UEFA Euro, Copa América, African Cup of Nations) from 2010-2025.

## Key Findings

### Historical Insights
- Average goals per World Cup match has ranged from 2.2 to 5.4
- Home advantage exists but is reduced in neutral venue tournaments
- Penalty shootouts occur in ~5% of knockout matches

### 2026 Predictions
- 48-team format will create more competitive diversity
- Traditional powerhouses still favored but with increased upset potential
- Teams with 70%+ recent win rates emerge as top contenders

### Model Performance
- Best model accuracy: ~55-65% on test set
- Feature importance: Team win rate > goal difference > goals per match
- Predicting draws remains challenging (inherent uncertainty in soccer)

## Project Structure

```
hex-a-thon/
├── data/
│   ├── raw/              # Original CSV datasets
│   └── processed/        # Cleaned and feature-engineered data
├── notebooks/
│   ├── 01_fifa_world_cup_analysis.ipynb  # Full ML pipeline
│   └── 02_quick_insights.ipynb            # Interactive visualizations
├── models/               # Saved ML models and scalers
├── docs/                 # Documentation
└── .github/
    └── copilot-instructions.md
```

## Getting Started

### Prerequisites
```bash
python 3.12+
pandas, numpy, scikit-learn, matplotlib, seaborn, plotly, joblib
```

### Installation
```bash
# Clone or navigate to project directory
cd hex-a-thon

# Install dependencies
pip install pandas numpy scikit-learn matplotlib seaborn plotly joblib
```

### Running the Analysis
1. Open `notebooks/01_fifa_world_cup_analysis.ipynb` for full ML pipeline
2. Open `notebooks/02_quick_insights.ipynb` for quick visualizations
3. Run cells sequentially to reproduce analysis

## Hex Platform Features

This project is designed for seamless transfer to Hex:

### Interactive Elements
- **Dynamic team selectors** for custom matchup predictions
- **Date range filters** for historical analysis
- **Tournament filters** for focused insights

### Semantic Layer Opportunities
- Team performance metrics as computed columns
- Tournament-level aggregations
- Time-based rolling statistics

### AI Thread Prompts
- "Which team has the best chance of winning in 2026?"
- "How has scoring changed in World Cups over time?"
- "Compare Brazil vs Argentina based on recent performance"
- "What's the impact of the 48-team format?"

## Visualizations

- **Team Performance Rankings**: Horizontal bar charts of win rates
- **Historical Trends**: Dual-axis time series of goals and matches
- **Top Scorers**: All-time goal-scoring leaders
- **Match Predictions**: Probability distributions for matchups
- **Confusion Matrices**: Model performance visualization

## Next Steps for Hex

1. **Upload notebooks** to Hex workspace
2. **Create data app** with interactive team selection
3. **Build Hex Threads** for conversational analytics
4. **Add input parameters** for custom date ranges and tournaments
5. **Enhance visualizations** with Hex's native charting
6. **Document methodology** in project overview

## Hackathon Deliverables

- Data analysis and feature engineering
- Machine learning prediction models
- Interactive visualizations
- Public Hex project (to be published)
- Demo video (≤3 minutes)
- Project overview document

##  Key Insights for Demo

1. **The 48-Team Revolution**: How expansion changes dynamics
2. **Data-Driven Favorites**: Top 5 contenders based on recent performance
3. **Historical Patterns**: 150 years of data reveals scoring trends
4. **Prediction Confidence**: Model accuracy and limitations
5. **Interactive Exploration**: Hex AI enables natural language queries

## Resources

- [Hex Documentation](https://docs.hex.tech)
- [FIFA World Cup History](https://www.fifa.com/fifaplus/en/tournaments/mens/worldcup)
- [Dataset Sources](https://github.com/martj42/international_results)
