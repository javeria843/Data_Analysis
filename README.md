**📊 freeCodeCamp Forum Page Views Analysis**
This project performs a comprehensive data visualization of daily page views on the freeCodeCamp forum from May 2016 to December 2019. It includes line plots, bar plots, and box plots to uncover trends, seasonality, and distribution patterns in user engagement.

📁 Dataset
Source: fcc-forum-pageviews.csv

Columns:

date: Timestamp of daily records

value: Number of page views

Outliers are removed using the 2.5th and 97.5th percentiles to ensure cleaner visualizations.

📈 Visualizations
1. Line Plot — Daily Page Views
Displays the overall trend of forum activity over time.

X-axis: Date

Y-axis: Page Views

Purpose: Highlights long-term trends and fluctuations.

2. Bar Plot — Monthly Averages by Year
Shows average page views per month across different years.



**🌊 Sea Level Rise Analysis**
This project visualizes historical sea level data from 1880 to 2013 using regression analysis and scatter plots. It highlights long-term trends and recent acceleration in sea level rise based on CSIRO-adjusted measurements.

📁 Dataset
Source: epa-sea-level.csv

Columns:

Year: Observation year

CSIRO Adjusted Sea Level: Sea level in inches (adjusted)

Lower/Upper Error Bound: Confidence interval bounds

NOAA Adjusted Sea Level: Additional measurements (NaN for early years)

📊 Visualizations
1. Scatter Plot — Historical Sea Level
X-axis: Year

Y-axis: CSIRO Adjusted Sea Level

Purpose: Shows raw data points from 1880 to 2013.

2. Linear Regression — Full Dataset
Red Line: Best-fit line from 1880 to 2013

Purpose: Projects sea level rise trend through 2050.

3. Linear Regression — Post-2000 Data
Green Line: Best-fit line from 2000 onward

Purpose: Highlights recent acceleration in sea level rise.

🛠️ Technologies Used
Python

Pandas

Matplotlib

SciPy (linregress)

Google Colab

🚀 How to Run
Upload epa-sea-level.csv via the Colab file upload widget.

Execute all cells to generate the plot.

The final visualization is saved as sea_level_plot.png.

📌 Notes
Two regression lines are plotted to compare historical vs. recent trends.

NOAA data is not used due to missing values in early years.

The legend warning is due to missing labels on plot lines — can be fixed by adding label='...' to each plt.plot() call.

X-axis: Year

Bars: Monthly averages

Purpose: Reveals seasonal patterns and year-over-year changes.

3. Box Plots — Yearly & Monthly Distributions
Two box plots side-by-side:

Left: Year-wise distribution (trend analysis)

Right: Month-wise distribution (seasonality)

Purpose: Visualizes spread, median, and outliers in page views.

🛠️ Technologies Used
Python

Pandas

Matplotlib

Seaborn

Google Colab

🚀 How to Run
Upload fcc-forum-pageviews.csv via the Colab file upload widget.

Execute all cells to generate the visualizations.

Ensure the runtime is active and the upload cell is rerun if needed.

📌 Notes
Data is preprocessed to remove statistical outliers.

Month names are ordered chronologically for accurate bar plots.

Box plots are sorted to reflect calendar months.
