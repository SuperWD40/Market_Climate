# Risk and Reward Climate Indicator

## Overview
This project provides a visualization tool for analyzing risk and reward indicators over time using scatter plots. The function `mc()` generates a scatter plot where data points are color-coded by year, helping to visualize trends and shifts in the dataset.

## Features
- Generates scatter plots with historical data color-coded by year
- Highlights the most recent data point for better trend identification
- Automatically adjusts axis limits for centered visualization
- Displays mean values with vertical and horizontal reference lines

## Installation
Ensure you have Python installed along with the required dependencies. You can install them using:

```bash
pip install matplotlib seaborn numpy pandas
```

## Usage
```python
import pandas as pd
from your_script import mc

# Load your data (Ensure it has a DateTime index)
df = pd.read_csv('your_data.csv', index_col=0, parse_dates=True)

# Generate the plot
mc(df, x_value='risk_metric', y_value='reward_metric')
```

## Parameters
- `df`: Pandas DataFrame containing the data
- `x_value`: Column name for the x-axis metric
- `y_value`: Column name for the y-axis metric
- `show` (default=True): If True, displays the plot; if False, saves the plot to a temporary file

## Example Output
The generated plot will show:
- A scatter plot with color-coded years
- A reference point for the latest data
- Vertical and horizontal lines representing mean values

## Author
This repository has been created by Mattéo Bernard

