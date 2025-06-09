# AIP-INTEGRATION-AND-DATA-VISUALIZATION

COMPANY NAME  :CODTECH ITT

NAME          :ROHITH.B

INTERN ID     :CT04DG566

DURATION      :08-06-2025 TO 08-07-2025

MENTOR NAME   :NEELA SANTHOSH KUMAR

🔍 Code Description

🔹 1. Import Libraries

import pandas as pd
import matplotlib.pyplot as plt

pandas is used for handling tabular data as DataFrames.

matplotlib.pyplot is used to create visualizations like line plots, bar charts, and pie charts.



---

🔹 2. Create a Sample Dataset

data = {
    'Day': ['Mon', 'Tue', 'Wed', 'Thu', 'Fri', 'Sat', 'Sun'],
    'Sales': [200, 150, 300, 280, 500, 700, 650]
}

A dictionary data is created with two keys:

'Day': Days of the week

'Sales': Corresponding sales values for each day




---

🔹 3. Convert to DataFrame

df = pd.DataFrame(data)

Converts the dictionary into a pandas DataFrame named df.

This structure is easier to work with for analysis and visualization.



---

🔹 4. Set Visualization Style

plt.style.use('ggplot')

Sets a clean and attractive plot style called 'ggplot'.



---

🔹 5. Line Plot

plt.figure(figsize=(8, 5))
plt.plot(df['Day'], df['Sales'], marker='o', linestyle='-', color='blue')
plt.title('Daily Sales Line Plot')
plt.xlabel('Day')
plt.ylabel('Sales')
plt.grid(True)
plt.tight_layout()
plt.show()

Draws a line plot showing sales trends over the week.

marker='o' adds circular markers at data points.

linestyle='-' connects the points with lines.

color='blue' gives the line a blue color.



---

🔹 6. Bar Chart

plt.figure(figsize=(8, 5))
plt.bar(df['Day'], df['Sales'], color='green')
plt.title('Daily Sales Bar Chart')
plt.xlabel('Day')
plt.ylabel('Sales')
plt.tight_layout()
plt.show()

Creates a bar chart comparing sales per day.

Each bar height represents the sales value for that day.

color='green' colors the bars green.



---

🔹 7. Pie Chart

plt.figure(figsize=(6, 6))
plt.pie(df['Sales'], labels=df['Day'], autopct='%1.1f%%', startangle=90)
plt.title('Sales Distribution Pie Chart')
plt.tight_layout()
plt.show()

Creates a pie chart to show the proportion of sales per day.

labels=df['Day']: Assigns labels to each slice.

autopct='%1.1f%%': Shows percentage values with 1 decimal place.

startangle=90: Rotates the pie chart for better orientation.



---

✅ Summary

This code demonstrates how to:

Prepare tabular data using pandas.

Visualize the data using different types of plots:

Line plot (for trend)

Bar chart (for comparison)

Pie chart (for proportion)


Use matplotlib styling and layout options to improve the visual appeal.
