# Affordable Air Travel Prediction Model

## Overview
This project analyzes and predicts commercial airline ticket prices within the United States using various machine learning techniques. The models achieve predictions within 10% accuracy for domestic flights using nearly 115,000 data points spanning multiple airlines, destinations, and passenger volumes.

## Features
- Airfare price prediction based on route information
- Clustering analysis of price patterns
- Random Forest and Neural Network prediction models
- Interactive tool for price predictions and budget-based recommendations
- Comprehensive data visualization

## Dataset
Primary data source: Bureau of Transportation Statistics
- 114,000 cleaned records (from initial 624,000)
- Data range: 2003-2023
- Key attributes:
  - Carrier (IATA code)
  - Origin and destination cities
  - Distance
  - Passenger numbers
  - Temporal data (year/quarter)

## Models
1. K-means Clustering
   - Groups similar routes and identifies pricing patterns
   - Outlier detection using z-scores

2. Random Forest
   - R² score: 0.75
   - MAPE: 12.93%
   - Key features: distance, year, market share

3. Neural Network
   - Architecture: 512-256-128 neurons
   - MAPE: 8.97%
   - MSE: 683.59
   - R²: 0.844

## Usage
The main tool can be found at the bottom of `main.ipynb`. Users can:
1. Input origin city
2. Input destination city
3. Set budget
4. Receive:
   - Price predictions
   - Budget feasibility analysis
   - Alternative destination suggestions

## Key Findings
- Airfares are primarily influenced by distance and year
- Markets with higher competition tend to have lower prices
- Third quarter typically offers better pricing
- Identified most/least expensive destinations and carriers

## Limitations
- Model accuracy decreases for:
  - International routes
  - Routes with very low passenger counts
  - Uncommon city pairs
  - Long-distance flights

## Future Improvements
- Expand dataset to include international flights
- Incorporate additional features:
  - Layover times
  - Seasonal demand
  - Economic indicators
- Implement more advanced prediction models
- Enhanced cross-validation techniques

## Contributors
- W. Avery Yeats
- Logan Schottland
- Devin Rocha
- Jaden Feldman