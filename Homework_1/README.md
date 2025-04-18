**Overview**
This notebook analyzes U.S. aircraft inventory data from 2006 to 2023 using a dataset provided by the Bureau of Transportation Statistics. The project includes missing data handling, data cleaning, variable transformations, feature engineering, and visualizations. It focuses on identifying data issues, standardizing fields, analyzing aircraft size groups, and visualizing operational and status trends. \\

**Running Code**
You can run the notebook using Jupyter Notebook, VSCode, or Google Colab. Make sure the dataset file (T_F41SCHEDULE_B43.csv) is located in the same directory as the notebook. There is no need to install any additional packages—standard libraries like pandas, numpy, matplotlib, seaborn, and scipy are used throughout. \\

**Expected Output**
*Part 1: Missing Data*
This section explores missing values in columns like MANUFACTURE_YEAR, CAPACITY_IN_POUNDS, NUMBER_OF_SEATS, CARRIER, and AIRLINE_ID. You’ll see several table outputs showing missing rows and how values were imputed using group-based logic or external lookups. \\

*Part 2: Data Standardization*
This part standardizes and cleans text fields like MANUFACTURER, MODEL, OPERATING_STATUS, and AIRCRAFT_STATUS. Outputs include .value_counts() tables and confirmation of cleaned string formats. No plots are generated in this section. \\

*Part 3: Final Cleaning*
Remaining missing values are dropped from the dataset. A short summary is printed showing the number of rows removed after cleaning.

*Part 4: Histograms and Box-Cox Transformation*
This section evaluates the skewness of NUMBER_OF_SEATS and CAPACITY_IN_POUNDS using histograms and applies the Box-Cox transformation. It includes four histograms (before and after) and skewness values before and after transformation.

*Part 5: Feature Engineering and Visualization*
A new SIZE category is created based on the quartiles of seat count. The notebook ends with two stacked bar charts showing proportions of OPERATING_STATUS and AIRCRAFT_STATUS across different size groups.
