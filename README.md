# 🏏 T20 Men's World Cup Cricket Analytics Dashboard

## 📊 Project Overview

A comprehensive cricket analytics project that leverages web scraping, data transformation, and business intelligence to analyze T20 Men's World Cup player performance data. This project demonstrates end-to-end data pipeline development from raw data extraction to interactive dashboard creation.

## 🎯 Key Achievements

- **Automated Data Collection**: Scraped comprehensive player statistics from ESPNCricInfo using Beautiful Soup and Bright Data
- **Data Engineering**: Transformed complex JSON structures into clean, analysis-ready CSV files
- **Feature Engineering**: Created derived metrics including player dismissal status and performance indicators
- **Statistical Analysis**: Applied advanced criteria to identify top-performing batsmen and bowlers
- **Business Intelligence**: Developed interactive Power BI dashboards for stakeholder insights

## 🛠️ Technologies Used

- **Web Scraping**: Beautiful Soup, Bright Data
- **Data Processing**: Python, Pandas, NumPy
- **Data Cleaning**: Regular Expressions (regex)
- **Visualization**: Power BI
- **Development Environment**: Jupyter Notebook

## 📁 Project Structure

```
cricket-analytics/
│
├── t20_json_files/           # Raw JSON data from web scraping
│   ├── t20_wc_match_results.json
│   ├── t20_wc_batting_summary.json
│   ├── t20_wc_bowling_summary.json
│   └── t20_wc_player_info.json
│
├── t20_csv_files/            # Processed CSV files
│   ├── match_summary.csv
│   ├── batting_summary.csv
│   ├── bowling_summary.csv
│   └── player_summary.csv
│
├── data_preprocessing.ipynb   # Data transformation notebook
├── power_bi_dashboard.pbix   # Interactive dashboard
└── README.md                  # Project documentation
```

## 🔄 Data Pipeline

### 1. Data Extraction
- Scraped T20 World Cup data from ESPNCricInfo
- Collected match results, batting statistics, bowling statistics, and player information
- Utilized Bright Data for enhanced scraping capabilities

### 2. Data Transformation
- **Match Summary Processing**:
  - Extracted 45 matches with 7 key attributes
  - Created unique match IDs for relational database structure
  
- **Batting Summary Enhancement**:
  - Processed batting records with 10+ metrics per player
  - Added "out/not_out" status using lambda functions
  - Cleaned player names using regex patterns
  
- **Bowling Summary Analysis**:
  - Captured 500 bowling records across all matches
  - Maintained detailed economy rates and wicket statistics
  
- **Player Information Normalization**:
  - Standardized 219 player profiles
  - Cleaned special characters from names
  - Preserved batting/bowling styles and playing roles

### 3. Feature Engineering
- Created match-level aggregations
- Calculated derived metrics:
  - Strike rates for batsmen
  - Economy rates for bowlers
  - Wicket percentages
  - Batting averages

## 📈 Key Performance Metrics

The analysis focused on identifying elite players based on:

### Top Batsmen Criteria
- Strike Rate > 140
- Batting Average > 30
- Minimum balls faced threshold
- Boundary percentage analysis

### Top Bowlers Criteria
- Economy Rate < 8.5
- Wicket percentage > 15%
- Dot ball percentage
- Death over specialist identification

## 🎨 Power BI Dashboard Features

- **Interactive Filters**: Team, match, and player selection
- **Performance Metrics**: Real-time calculation of key statistics
- **Comparative Analysis**: Head-to-head player comparisons
- **Trend Analysis**: Performance over tournament progression
- **Visual Reports**: Heat maps, scatter plots, and performance matrices

## 🚀 Getting Started

### Prerequisites
```bash
pip install pandas numpy beautifulsoup4 jupyter
```

### Running the Analysis
1. Clone the repository
2. Open `data_preprocessing.ipynb` in Jupyter Notebook
3. Run all cells to process the JSON files into CSV format
4. Open the Power BI dashboard file for interactive visualizations

## 💡 Key Insights

- Identified performance patterns across different match conditions
- Discovered correlation between strike rates and match outcomes
- Analyzed bowling economy variations in powerplay vs death overs
- Created player performance indices for team selection strategies

## 🔮 Future Enhancements

- [ ] Real-time data pipeline integration
- [ ] Machine learning models for performance prediction
- [ ] Automated report generation
- [ ] API development for data access
- [ ] Extended historical data analysis

## 📊 Sample Analysis Output

The project successfully processed:
- **45** T20 World Cup matches
- **500+** individual batting performances
- **500** bowling spell records
- **219** unique player profiles

## 🤝 Contributing

Contributions are welcome! Please feel free to submit a Pull Request.

---

*This project demonstrates proficiency in data engineering, web scraping, data transformation, and business intelligence dashboard development.*
