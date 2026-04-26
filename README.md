# Experiment-18

## Aim
To explore statistical and specialized data visualization techniques using Python libraries to analyze a generated dataset, uncover distributions, and visualize relationships between multiple variables.

## Theory
Data visualization is the graphical representation of data that helps uncover trends, relationships, and proportions. This experiment utilizes Python libraries—Pandas and NumPy for data manipulation, alongside Matplotlib and Seaborn for rendering visualizations. A dataset is typically structured with categorical data (e.g., Category) and corresponding numerical metrics (e.g., Value, Sales, and Profit).

The following specialized statistical graphs are utilized to understand different data perspectives:

1. Single Variable Area Plot
Purpose: An area plot shows how quantitative data develops across categories by filling the area below the line.

Implementation Details: A standard area plot is created using plt.fill_between to map a metric across categories. It utilizes fill colors with transparency (alpha) to maintain visibility of the grid lines, and includes custom axes labels.

2. Comparative Area Plot
Purpose: Used to compare multiple quantitative variables across categories simultaneously.

Implementation Details: Overlays two or more variables (like Sales and Profit) against categories. Different colors are used for each metric, with transparency (alpha) set to ensure the overlapping areas remain visible.

3. Pie Chart
Purpose: A circular graphic divided into slices to illustrate numerical proportions.

Implementation Details: Plotted using plt.pie() to visualize the proportion of a metric for each respective category label. Visual encoding includes the autopct parameter to display exact percentage values inside each slice.

4. Donut Chart
Purpose: A variation of a pie chart with a blank center, providing a cleaner way to visualize proportions.

Implementation Details: Constructed by first generating a standard pie chart and then overlaying a white circular shape (plt.Circle) with a specific radius at the center coordinates to create the "donut" hole.

5. Box Plot (Box-and-Whisker Plot)
Purpose: A standardized way of displaying the distribution of data based on a five-number summary: minimum, first quartile (Q1), median, third quartile (Q3), and maximum. It is highly effective for identifying outliers.

Implementation Details: Typically implemented using sns.boxplot() or plt.boxplot(). It allows for visualizing the spread and skewness of numerical variables (like Sales or Profit) either as a whole or broken down across different Category variables. The "whiskers" show the range of the data, while points outside this range are plotted individually as outliers.

6. Bubble Chart
Purpose: An extension of the scatter plot that allows you to visualize three dimensions of data at once. The x and y axes represent two variables, and the size of the "bubble" represents the third variable.

Implementation Details: Created using plt.scatter(). Two numerical variables (e.g., Sales and Profit) are plotted on the X and Y axes, while a third numerical metric (e.g., Value) is passed to the size parameter (s). Transparency (alpha) is often applied so that overlapping bubbles can still be distinguished.

7. Heat Map
Purpose: A 2D graphical representation of data where the individual values contained in a matrix are represented as colors. It is exceptional for finding patterns, variance, and correlations between multiple numerical variables.

Implementation Details: Commonly generated using Seaborn's sns.heatmap(). A correlation matrix (e.g., df.corr()) is first calculated for the numerical columns. The heatmap maps these correlation values to a color gradient (colormap like cmap='coolwarm'). The annot=True parameter is usually added to display the exact numerical correlation coefficients within each cell.

## Conclusion
The experiment successfully demonstrates the application of Python libraries (Pandas, NumPy, Matplotlib, Seaborn) to generate specialized statistical charts and apply advanced visual encodings. By implementing area plots, pie/donut charts, box plots, bubble charts, and heat maps, tabular data is transformed into highly analytical graphical representations.
