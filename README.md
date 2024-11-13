# Data Visualization in Python

This repository contains a collection of Python code snippets demonstrating various data visualization techniques using popular libraries like **Matplotlib**, **Seaborn**, and **Plotly**. The goal is to show how these libraries can be used to create meaningful and visually appealing representations of data.

## Libraries Used

The following libraries are employed to generate different types of visualizations:

- **Matplotlib**: A basic and powerful plotting library for creating 2D visualizations.
- **Seaborn**: Built on top of Matplotlib, Seaborn simplifies the creation of complex statistical visualizations.
- **Plotly**: Provides interactive plots, ideal for web-based data visualization.

## Project Structure

The repository contains several Python scripts, each demonstrating a specific type of visualization:

- `matplotlib_visualizations.py`: Examples of creating basic and advanced visualizations using Matplotlib (e.g., line plots, histograms, pie charts).
- `seaborn_visualizations.py`: Demonstrations of statistical visualizations using Seaborn (e.g., heatmaps, pair plots, violin plots).
- `plotly_visualizations.py`: Examples of creating interactive visualizations with Plotly (e.g., scatter plots, 3D plots).

## Example Datasets

Some example datasets used throughout the repository are:

- **Iris Dataset**: A popular dataset for classification tasks, included in Seaborn and Plotly.
- **Tips Dataset**: A dataset that contains restaurant tips data, available in Seaborn.
- **Custom Datasets**: You can replace the built-in datasets with your own data by modifying the code in the scripts.

## Basic Usage Examples

### 1. Matplotlib

```python
import matplotlib.pyplot as plt

# Sample Data
x = [1, 2, 3, 4]
y = [10, 20, 25, 30]

# Line Plot
plt.plot(x, y)
plt.title("Line Plot")
plt.xlabel("X-axis")
plt.ylabel("Y-axis")
plt.show()
```

### 2. Seaborn

```python
import seaborn as sns
import matplotlib.pyplot as plt

# Load sample dataset
tips = sns.load_dataset("tips")

# Scatter Plot
sns.scatterplot(data=tips, x="total_bill", y="tip", hue="day")
plt.title("Seaborn Scatter Plot")
plt.show()
```

### 3. Plotly

```python
import plotly.express as px

# Load sample data
df = px.data.iris()

# Interactive Scatter Plot
fig = px.scatter(df, x="sepal_width", y="sepal_length", color="species")
fig.show()
```
## Advanced Features

This project also explores more advanced features of each visualization library:

- **Matplotlib**: Customizing plots with colors, styles, and annotations.
- **Seaborn**: Creating complex visualizations such as pair plots, heatmaps, and facet grids.
- **Plotly**: Adding interactive components like tooltips, legends, and subplots.
  
## Usage in Real-World Projects

Data visualization is critical in various real-world applications, such as:

- **Business Analytics**: Visualizing sales data, customer behavior, and market trends to support decision-making.
- **Healthcare**: Using visualizations to represent trends in patient data, disease progression, or treatment outcomes.
- **Education**: Visualizing student performance, demographics, and academic progress to drive improvements in teaching methods.
- **Social Media Analytics**: Analyzing user engagement, posts, and interactions to understand social trends and user behavior.

This repository can serve as a foundation for building data visualization solutions in these domains.
