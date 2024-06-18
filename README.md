
# Comprehensive Analysis and Prediction of Built-up Area Trends

This repository contains a comprehensive analysis of historical urban area data and predictions for future trends. The analysis utilizes higher-end models, including LSTM for time-series prediction, and separates the analysis between BCE (Before Common Era) and AD (Anno Domini) periods.

## Table of Contents

- [Comprehensive Analysis and Prediction of Built-up Area Trends](#comprehensive-analysis-and-prediction-of-built-up-area-trends)
  - [Table of Contents](#table-of-contents)
  - [Project Overview](#project-overview)
  - [Dataset](#dataset)
  - [Installation](#installation)
  - [Usage](#usage)
  - [Analysis](#analysis)
    - [Data Preprocessing](#data-preprocessing)
    - [PCA Analysis](#pca-analysis)
    - [LSTM Prediction](#lstm-prediction)
  - [Results](#results)
  - [Conclusion](#conclusion)
  - [Contributing](#contributing)
  - [License](#license)

## Project Overview

This project aims to analyze the historical trends in built-up areas globally and predict future trends using advanced machine learning models. The analysis is conducted separately for BCE and AD periods to provide a clear understanding of historical and modern urban development.

## Dataset

The dataset used in this project is an updated and expanded version of the History Database of the Global Environment (HYDE, v3.3). It covers the period from 10,000 BCE to 2023 CE and includes various categories of land use and population data.

The dataset can be found in Kaggle: [Urban area over](https://www.kaggle.com/datasets/willianoliveiragibin/urban-area-over)

## Installation

To run this project, you need to have Python installed along with the following packages:

- pandas
- numpy
- matplotlib
- seaborn
- scikit-learn
- tensorflow

You can install the necessary packages using pip:

```sh
pip install pandas numpy matplotlib seaborn scikit-learn tensorflow
```

## Usage

Clone the repository:

```sh
git clone https://github.com/debjit-mandal/urban-developments-trends-analysis.git
cd urban-developments-trends-analysis
```

Run the Jupyter notebook to see the analysis and predictions:

```sh
jupyter notebook Analysis.ipynb
```

## Analysis

### Data Preprocessing

- The dataset is loaded and preprocessed to handle missing values and convert necessary fields to numeric types.
- The 'Year' column is used to distinguish between BCE and AD periods, and a new feature 'Built-up Area per Year' is created.

### PCA Analysis

- Principal Component Analysis (PCA) is performed separately for BCE and AD data to visualize the variance in built-up areas over time.

### LSTM Prediction

- LSTM (Long Short-Term Memory) networks are used to predict future trends in built-up areas.
- The data is normalized, and sequences are created for LSTM input.
- Separate models are trained for BCE and AD data, and future predictions are generated for the next 100 years.

## Results

The analysis provides insights into the historical trends in urban development and predicts future built-up area trends. The results are visualized using line plots and PCA scatter plots.

## Conclusion

This project demonstrates the application of advanced machine learning techniques to analyze and predict trends in historical data. By separating the analysis for BCE and AD periods, we gain a clearer understanding of the differences in urban development over time.

## Contributing

Contributions are welcome! Please fork this repository and submit a pull request for any improvements or bug fixes.

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.
