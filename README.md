
# HVAC Data Analysis and Anomaly Detection

This project focuses on the analysis of HVAC (Heating, Ventilation, and Air Conditioning) data. The project includes data preprocessing, visualization, and anomaly detection using various techniques.

## Project Structure

* **Data Preprocessing**: Cleaning and preparing the HVAC dataset for analysis.
* **Visualization**: Plotting various aspects of the data, including relative humidity, to understand trends and detect outliers.
* **Anomaly Detection**: Implementing methods to identify anomalies in the relative humidity data.

## Notebooks

* **HVAC.ipynb**: The main notebook that contains the entire workflow, from data loading to anomaly detection and visualization.

## Dependencies

To run this project, you need the following Python libraries:

* `pandas`
* `numpy`
* `matplotlib`
* `scikit-learn` (for anomaly detection models)

You can install the necessary packages using the following command:

```bash
pip install pandas numpy matplotlib scikit-learn
```

## Usage

1. **Clone the repository**:

```bash
git clone https://github.com/yourusername/hvac-anomaly-analysis.git
cd hvac-anomaly-analysis
```

2. **Run the notebook**: Open `HVAC.ipynb` in Jupyter Notebook or JupyterLab and execute the cells to reproduce the analysis.

## Data Definitions

* **T_supply**: Temperature supply
* **T_return**: Temperature return
* **SP_return**: Temperature set points of the return air
* **T_Saturation**: Saturation temperature in the humidifier
* **T_Outdoor**: Temperature outdoor
* **RH_Supply**: Relative humidity supply (%)
* **RH_Return**: Relative humidity return (%)
* **RH_Outdoor**: Relative humidity outdoor(%)

## HVAC Data Combinations and Their Insights

### 1. Temperature Control

| Data Combination | Answer Provided |
|-------------------|-----------------|
| T_Supply vs T_Return | Efficiency of heat exchange and distribution |
| T_Supply vs T_Outdoor | System's ability to respond to outdoor temperature changes |
| T_Saturation vs (T_Supply, T_Return) | Performance of cooling coil and dehumidification process |

### 2. Humidity Control

| Data Combination | Answer Provided |
|-------------------|-----------------|
| RH_Supply vs RH_Return | Effectiveness of moisture removal or addition |
| RH_Supply vs RH_Outdoor | System's ability to control indoor humidity relative to outdoor conditions |

### 3. Energy Efficiency

| Data Combination | Answer Provided |
|-------------------|-----------------|
| Energy vs (T_Supply - T_Return) | Energy efficiency of cooling/heating processes |
| Power vs T_Outdoor | Appropriateness of power consumption relative to outdoor temperature |

### 4. System Performance

| Data Combination | Answer Provided |
|-------------------|-----------------|
| SP_Return vs T_Return | System's ability to meet and maintain setpoint temperatures |

### 5. Complex System Behavior

| Data Combination | Answer Provided |
|-------------------|-----------------|
| T_Supply, RH_Supply, Energy | Overall system performance in managing temperature, humidity, and energy use |
| T_Outdoor, T_Supply, Power | System's efficiency and response to varying outdoor conditions |

### 6. Time-Based Patterns

| Data Combination | Answer Provided |
|-------------------|-----------------|
| Any parameter vs Time of Day | Daily patterns in system behavior and potential scheduling issues |
| Any parameter vs Day of Week | Weekly patterns in system performance and occupancy-related effects |

### 7. Anomaly Detection

| Data Combination | Answer Provided |
|-------------------|-----------------|
| Any parameter vs Its Historical Range | Identification of unusual behavior in individual system components |
| Multiple parameters vs Their Expected Relationships | Detection of complex anomalies affecting multiple aspects of the system |

## Contributing

If you'd like to contribute to this project, feel free to open a pull request or report any issues.


## Authors

- [@iamaber](https://github.com/iamaber)
