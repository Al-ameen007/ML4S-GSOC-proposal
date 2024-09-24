# Thermonuclear Supernova Classification via Multi-Wavelength Signatures

## Overview

This project focuses on classifying thermonuclear supernovae based on their multi-wavelength signatures using a variety of observable and physical parameters. The dataset includes numerical data related to supernova parameters such as **vmax**, **tao**, and **Φ300**. The project explores trends, relationships, and correlations between these parameters through visualization and machine learning techniques.

## Workflow

### 1. Data Import and Preprocessing
- The dataset is read into a **pandas DataFrame**, and its structure is analyzed.
- No missing values were identified, eliminating the need for data cleaning. However, **scaling** is necessary due to varying ranges among the parameters, particularly for **tao**.

### 2. Exploratory Data Analysis (EDA)
- A **correlation matrix** and **pair plots** were generated to explore relationships between observable parameters. 
- Key findings:
  - **tao** and **Φ300** show periodicity.
  - There are strong correlations between **Φ300** and **tao**, and the data can be grouped into four distinct clusters.
  - **tao** and **vmax** exhibit normal distributions, while **Φ300** shows a wider range.

### 3. Parallel Coordinates Plot
- A parallel coordinates plot was used to visualize the relationships between observable parameters and numerical physical parameters.
- Observations:
  - **tao** has a wider range compared to other parameters, necessitating scaling.
  - Although the parameters are numerical, they appear to take on discrete values.
  - Some physical parameters, such as **Initial 56Ni radial distribution** and **Initial SNeIa mass distribution**, show compact relationships with **tao** and **vmax** but are more spread out with **Φ300**.

### 4. Insights from Scatter Plots
- **Explosion energy** shows little to no correlation with other parameters.
- The **Initial SNeIa mass distribution** and **Initial 56Ni radial distribution** flags are more closely related to observable parameters like **tao** and **vmax**, while **Φ300** presents a wider spread.

## Results
The project provided insights into the relationships between various observable and physical parameters, which will assist in developing more sophisticated models for thermonuclear supernova classification.
