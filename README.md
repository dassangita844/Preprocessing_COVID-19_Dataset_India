
# Impact of Comprehensive Data Preprocessing on Predictive Modelling of COVID-19 Mortality

### Authors: **Sangita Das & Subhrajyoti Maji**

## Overview

This repository contains a Jupyter notebook that demonstrates the impact of comprehensive data preprocessing on the predictive modeling of COVID-19 mortality. The project focuses on leveraging advanced preprocessing techniques to improve the reliability and accuracy of predictions, comparing the performance of various machine learning models trained on custom versus standard preprocessing pipelines.

## Objectives

- **Explore Computational Dependencies:** Examine relationships among dataset columns to accurately fill in missing values and address inconsistencies through custom computations.
- **Custom Preprocessing Pipeline:** Construct a tailored preprocessing pipeline that includes various custom transformers to clean, normalize, and enhance the raw data.
- **Impact Analysis:** Assess and compare the performance of multiple linear and non-linear models using custom preprocessing versus standard preprocessing, highlighting the benefits of detailed preprocessing steps.

## Data Source

The dataset used in this project is sourced from:

- **Our World in Data (OWID) COVID-19 Dataset**: Available at [Our World in Data](https://github.com/owid/covid-19-data/tree/master/public/data). The dataset provides comprehensive global data on COVID-19 cases, deaths, vaccinations, and other related metrics, serving as the foundation for the predictive modeling and analysis conducted in this notebook. When using this data, please cite as follows:

  > Edouard Mathieu, Hannah Ritchie, Lucas Rodés-Guirao, Cameron Appel, Charlie Giattino, Joe Hasell, Bobbie Macdonald, Saloni Dattani, Diana Beltekian, Esteban Ortiz-Ospina and Max Roser (2020) - "Coronavirus Pandemic (COVID-19)". Published online at OurWorldInData.org. Retrieved from: 'https://ourworldindata.org/coronavirus' [Online Resource]

## Installation

To run the notebook and reproduce the results, install the required Python packages:

```bash
!pip install pandas matplotlib seaborn ipywidgets plotly qgrid
```

## Repository Structure


```plaintext
├── data/
│   ├── original_india_data.csv                   # Original data for India from OWID
│
├── standard/                                  
│   ├── models/                                   # Trained models using the standard pipeline
│   ├── plots/                                    # Plots for learning curves and global outlier processing
│   ├── tables/                                                            
│   │   ├── feature_importance/                   # Feature importance tables from round 0 to 21
│   │   ├── feature_correlation_with_target.csv   # Correlation of features with the target variable
│   │   ├── standard_processed_india_data.csv     # Processed data after applying the standard preprocessing pipeline
│   │   ├── standard_results.csv                  # Results from models trained with standard preprocessing
│
├── custom/                                  
│   ├── models/                                   # Trained models using the custom pipeline
│   ├── plots/                                    # Plots for learning curves, computation and local outlier processing, and weekly pattern imputation
│   ├── tables/                                                             
│   │   ├── feature_importance/                   # Feature importance tables from round 0 to 18
│   │   ├── feature_correlation_with_target.csv   # Correlation of features with the target variable
│   │   ├── custom_processed_india_data.csv       # Processed data after applying the custom preprocessing pipeline
│   │   ├── custom_results.csv                    # Results from models trained with custom preprocessing
│
├── Enhanced_predictive.ipynb                     # Main notebook for preprocessing and modeling
├── README.md                                     # Project overview and instructions
└── LICENSE                                       # License information

```

## Notebook Structure

1. **Introduction**
   - Problem Overview
   - Objectives

2. **Setup**
   - Installation of required packages
   - Loading data

3. **Data Preprocessing**
   - Standard preprocessing pipeline
      - Handling missing values and outliers
      - Iterative feature selection

   - Custom preprocessing pipeline
      - Weekly pattern imputation
      - Local outlier processing
      - Computation processing
      - Iterative feature selection

4. **Modeling**
   - Training multiple machine learning models
   - Comparing models trained on custom vs. standard preprocessing

5. **Results and Analysis**
   - Performance metrics (Test RMSE, Test R², RMSE Variance)
   - Impact of preprocessing on model performance

6. **Conclusion**
   - Summary of findings

## Results

The notebook demonstrates that comprehensive data preprocessing significantly improves the performance of predictive models in terms of accuracy and reliability. Custom preprocessing pipelines that take into account specific dataset characteristics yield better results compared to standard approaches.

## Citation

If you use this code in your research, please cite the following paper:

> Das, S., & Maji, S. (2024). *Impact of Comprehensive Data Preprocessing on Predictive Modeling of COVID-19 Mortality*. Journal Name, Volume(Issue), pages. doi:xx.xxxx/xxxxx

## Usage

To use the notebook:

1. Clone the repository.
2. Install the necessary packages using the provided `pip` command.
3. Open the notebook in Jupyter and execute the cells to reproduce the results.

## Contributing

Contributions are welcome! If you have suggestions or improvements, feel free to open an issue or submit a pull request.

## License

This project is licensed under the MIT License.
