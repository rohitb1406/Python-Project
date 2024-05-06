### Project Description: Medical Data Visualizer
## Main Code:
- **Import Libraries**: The code imports necessary libraries including Pandas, Seaborn, Matplotlib, and NumPy.
- **Read Data**: It reads medical examination data from a CSV file (medical_examination.csv) into a Pandas DataFrame.
- **Add 'overweight' Column**: The code calculates the BMI (Body Mass Index) for each individual and adds an 'overweight' column indicating whether the person is overweight (1) or not (0).
- **Normalize Data**: It normalizes the 'cholesterol' and 'gluc' columns, converting values less than or equal to 1 to 0 and values greater than 1 to 1.
- **Draw Categorical Plot**: A function draw_cat_plot() is defined to draw a categorical plot (catplot) using Seaborn, displaying counts of various features split by cardiovascular disease status ('cardio').
  - It creates a DataFrame using pd.melt() to melt the DataFrame based on the specified variables.
  -The catplot is drawn using sns.catplot() to show the distribution of categorical variables.
  -The resulting plot is saved as 'catplot.png'.
## Test Module:
- **Unit Testing**: The code includes a test module (test_module.py) to test the functionality of the main code.
- **CatPlot Test Case**:
  - It tests the labels and the number of bars in the catplot.
  - Verifies that the xlabel is 'variable' and the ylabel is 'total'.
  - Checks if the number of bars in the plot is correct.
- **HeatMap Test Case**:
  - It tests the labels and the values displayed in the heatmap.
  - Verifies that the labels in the heatmap are correct.
  - Checks if the values displayed in the heatmap match the expected values.
## Conclusion:
The Medical Data Visualizer project provides insights into medical examination data using visualizations. It allows for easy analysis of factors like BMI, cholesterol, glucose levels, and lifestyle choices in relation to cardiovascular disease. With the inclusion of unit tests, the project ensures the correctness of the visualizations and the underlying data analysis.
