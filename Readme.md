# SpaceX Falcon 9 First Stage Landing Prediction

![SpaceX Falcon 9](https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBMDeveloperSkillsNetwork-DS0701EN-SkillsNetwork/api/Images/landing_1.gif)

## 📌 Project Overview

This repository contains the coursework and final deliverables for the **IBM Data Science Professional Certificate Capstone Project**.

The goal of this project is to predict whether the first stage of the SpaceX Falcon 9 rocket will land successfully. SpaceX advertises Falcon 9 rocket launches on its website with a cost of 62 million dollars; other providers cost upward of 165 million dollars each, much of the savings is because SpaceX can reuse the first stage. Therefore, if we can determine if the first stage will land, we can determine the cost of a launch. This information can be used if an alternate company wants to bid against SpaceX for a rocket launch.

**Note:** This project was completed as part of a grading requirement for the IBM Data Science Professional Certificate. The base curriculum and problem statement were designed by IBM, while the code implementation, analysis, model building, and conclusions were executed by **Muhammad Rayyan**.

## 📂 Repository Structure

The project is divided into several stages, represented by the following Jupyter Notebooks:

### 1. Data Collection
- **`1.jupyter-labs-spacex-data-collection-api.ipynb`**:  
  Collecting data from the SpaceX API, including launch details, booster versions, and payloads.
- **`2 -jupyter-labs-webscraping.ipynb`**:  
  Web scraping Falcon 9 launch records from Wikipedia using BeautifulSoup to supplement API data.

### 2. Data Wrangling
- **`3.labs-jupyter-spacex-Data wrangling.ipynb`**:  
  Cleaning the dataset, handling missing values, filtering for Falcon 9 launches, and creating binary classification labels for landing outcomes.

### 3. Exploratory Data Analysis (EDA)
- **`4. jupyter-labs-eda-sql-coursera_sqllite.ipynb`**:  
  Using SQL (SQLite) to query the dataset and extract insights regarding launch sites, payload masses, and success rates.
- **`5. jupyter-labs-eda-dataviz.ipynb`**:  
  Visualizing relationships between variables (e.g., Flight Number vs. Launch Site, Payload vs. Orbit) using Matplotlib and Seaborn.

### 4. Interactive Visual Analytics
- **`6.1 lab_jupyter_launch_site_location-Folium lab.ipynb`**:  
  Creating interactive maps using **Folium** to visualize launch sites and their proximity to coastlines, railways, and highways.
- **`6.2 spaceX Dash App.ipynb`**:  
  Building an interactive dashboard using **Plotly Dash** to allow users to filter launches by site and payload range to analyze success rates.

### 5. Machine Learning Prediction
- **`7. SpaceX_Machine_Learning_Prediction_Part_5.jupyterlite.ipynb`**:  
  Building and evaluating classification models to predict landing success.
  - **Models tested:** Logistic Regression, Support Vector Machine (SVM), Decision Tree, and K-Nearest Neighbors (KNN).
  - **Methods:** Data splitting, Standardization, Hyperparameter tuning using GridSearchCV.
  - **Best Model:** Decision Tree Classifier (approx. 88.89% accuracy on test data).

## 🛠 Technologies Used
- **Languages:** Python, SQL
- **Libraries:** Pandas, NumPy, Matplotlib, Seaborn, Scikit-Learn, Folium, Plotly, Dash, BeautifulSoup, Requests.
- **Tools:** Jupyter Notebooks, IBM Watson Studio (optional context).

## 📈 Key Findings
- **Launch Sites:** KSC LC-39A and VAFB SLC 4E have higher success rates compared to CCAFS SLC 40.
- **Orbits:** Low Earth Orbit (LEO) and ISS missions have higher success rates than GTO missions.
- **Payload:** Heavy payloads generally have a high success rate across specific orbits.
- **Trend:** Launch success rates have improved significantly over the years as SpaceX refined their technology.

## 👤 Author

**Muhammad Rayyan**  
- **GitHub:** [sayad1711](https://github.com/sayad1711/)

---
*Disclaimer: This project is for educational purposes as part of the IBM Data Science Professional Certificate.*