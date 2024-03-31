# Predicting Categories of Flight Delay Among Popular Airlines

### By Yssa Traore

**Table of Contents**
1. [Introduction and Problem Statement](#introduction-and-problem-statement)
2. [Categorization of Delays](#categorization-of-delays)
3. [Objective](#objective)
4. [Dataset Information](#dataset-information)
5. [Methodology](#methodology)
6. [Usage](#usage)
7. [Tech Stack](#tech-stack)


## Introduction and Problem Statement
In the aviation industry, flight delays are more than just inconveniences; they represent a significant challenge affecting operational efficiency and passenger satisfaction. The goal of this study is to develop a predictive model capable of categorizing flight delays into one of three distinct categories based on their duration: no delay, moderate delay, and lengthy delay. This classification is not arbitrary but is based on the real-world implications of delay durations on passengers' schedules and the operational logistics of airlines.

## Categorization of Delays
The delays are categorized as follows, based on the duration:
- **No Delay:** Delays of 10 minutes or less, typically negligible in impact.
- **Moderate Delay:** Delays ranging from 10 to 30 minutes, which can cause inconvenience.
- **Lengthy Delay:** Delays exceeding 30 minutes, often leading to significant disruptions.

The classification thresholds are determined using the 0.33 and 0.66 quantiles of the delay duration distribution within the dataset, providing a data-driven approach to understanding delay impacts.

## Objective
The primary objective is to apply machine learning techniques to predict the delay category of a given flight accurately. This predictive model aims to enhance communication and planning for airlines and improve the overall travel experience for passengers by providing insights into potential delays.

## Dataset Information
The analysis utilizes three key datasets:
- **Main Dataset (`DelayedFlights.csv`):** Contains comprehensive flight data including origin, day and time, month, taxi times, and more.
- **Carrier Data (`L_UNIQUE_CARRIERS.csv`):** Used to decode airline codes to names for better readability.
- **Airport Data (`L_AIRPORT.csv`):** Translates airport codes to names, aiding in interpretability.

These datasets include over 5,000 entries and are crucial for understanding and predicting flight delays.

## Methodology
The project employs several data visualization techniques, including Seaborn, Matplotlib, and histograms, to analyze the datasets. A Decision Tree model was chosen for its effectiveness in handling categorical data and its interpretability. The model analyzes factors such as departure and arrival times, flight distance, and taxi times to predict delays across more than 10,000 flights.

## Usage
To use this project for predicting flight delay categories, follow these steps:
1. Download the datasets mentioned above and place them in the designated data folder.
2. Install the necessary Python packages: pandas, numpy, matplotlib, seaborn, and scikit-learn.
3. Run the main analysis notebook to train the model and make predictions. Detailed instructions and comments within the notebook guide through the process.

## Tech Stack
This project leverages a variety of technologies and tools across data analysis, visualization, and machine learning development:
- **Programming Language:** Python 3
- **Data Analysis and Manipulation:** Pandas, NumPy, Scikit-learn
- **Data Visualization:** Matplotlib, Seaborn
- **Machine Learning:** Decision Trees Classifier
- **Development Environment:** Jupyter Notebooks
- **Version Control:** Git, GitHub
- **Dataset Storage and Management:** Local file storage

### Installation and Setup
Ensure Python 3.x is installed, along with Jupyter Notebooks. Install required Python libraries with pip:
```bash
pip install pandas numpy matplotlib seaborn scikit-learn jupyter
```
For version control, ensure Git is installed and clone the repository from GitHub.
