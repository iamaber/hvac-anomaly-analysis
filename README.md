# HVAC Anomaly Analysis

## Project Description and Overview

This project performs anomaly detection and analysis on HVAC (Heating, Ventilation, and Air Conditioning) system data to identify unusual patterns, equipment malfunctions, and energy efficiency issues. The analysis uses machine learning techniques to detect anomalies in HVAC performance data collected over multiple years.

### Key Features
- Time series analysis of HVAC sensor data
- Anomaly detection using statistical and machine learning methods
- Energy consumption pattern analysis
- Equipment performance monitoring
- Visualization of anomalies and trends

## Dataset Information

The analysis uses the `HVAC_NE_EC_19-21.csv` dataset which contains:
- **Time Period**: 2019-2021 HVAC system data
- **Location**: Northeast region energy consumption data
- **Data Types**: Temperature readings, energy consumption, system status indicators
- **Frequency**: Regular time-series measurements

### Data Structure
The dataset includes various HVAC system parameters such as:
- Timestamp information
- Temperature measurements (indoor/outdoor)
- Energy consumption metrics
- System operational status
- Environmental conditions

## Usage Examples

### Running the Analysis

1. **Open the Jupyter Notebook**:
   ```bash
   jupyter notebook HVAC.ipynb
   ```

2. **Execute the analysis cells** to:
   - Load and preprocess the HVAC data
   - Perform exploratory data analysis
   - Apply anomaly detection algorithms
   - Generate visualizations and reports

3. **View Results**:
   - Anomaly detection plots
   - Time series analysis charts
   - Statistical summaries
   - Performance metrics

### Key Analysis Steps
```python
# Load the dataset
df = pd.read_csv('HVAC_NE_EC_19-21.csv')

# Perform anomaly detection
anomalies = detect_hvac_anomalies(df)

# Visualize results
plot_anomaly_detection_results(df, anomalies)
```

## Analysis Results Summary

### Key Findings
- **Anomaly Detection**: Identified seasonal patterns and equipment performance issues
- **Energy Efficiency**: Analyzed consumption trends and identified optimization opportunities
- **System Performance**: Monitored HVAC system reliability and maintenance needs
- **Temporal Patterns**: Discovered daily, weekly, and seasonal operational patterns

### Insights Generated
- Peak energy consumption periods
- Equipment malfunction indicators
- Maintenance scheduling recommendations
- Energy efficiency improvement opportunities

### Visualizations
The analysis produces various charts and plots including:
- Time series plots of HVAC parameters
- Anomaly detection scatter plots
- Seasonal decomposition charts
- Energy consumption heatmaps

## Requirements

- Python 3.7+
- Jupyter Notebook
- pandas
- numpy
- matplotlib
- seaborn
- scikit-learn
- Additional dependencies as specified in the notebook

## Installation

1. Clone the repository
2. Install required packages:
   ```bash
   pip install -r requirements.txt
   ```
3. Launch Jupyter Notebook and open `HVAC.ipynb`

## Files Structure

```
hvac-anomaly-analysis/
├── HVAC.ipynb              # Main analysis notebook
├── HVAC_NE_EC_19-21.csv    # Dataset file
├── metadata.txt            # Dataset metadata
└── README.md              # This file
```
