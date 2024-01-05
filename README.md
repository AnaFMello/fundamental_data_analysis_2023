# fundamental_data_analysis_2023
## Ana Mello


# Task 1 - The Collatz conjecture



----------------------------------------
# Task 2 - Penguins data set



----------------------------------------

# Task 3 - Penguins data set probability distribution



----------------------------------------
# Task 4 - Coin Flipping Entropy
Suppose you are flipping two coins, each with a probability \( p \) of giving heads. The task is to plot the entropy of the total number of heads versus \( p \).

## Entropy Calculation

The entropy of a probability distribution is calculated using the formula:

\[ H(X) = - \sum_{i} p_i \log(p_i) \]

where \( p_i \) is the probability of the \( i \)-th outcome. In this case, the random variable \( X \) represents the total number of heads when flipping two coins.

The possible outcomes for \( X \) are:
- 0 heads
- 1 head
- 2 heads

The probabilities for these outcomes are:
\[ P(X=0) = (1-p)^2 \]
\[ P(X=1) = 2p(1-p) \]
\[ P(X=2) = p^2 \]

## Implementation

The provided Python script calculates the entropy for different values of \( p \) and plots the entropy against \( p \). The x-axis represents the probability \( p \) of getting heads on each coin, and the y-axis represents the entropy of the total number of heads.

## ```python
import matplotlib.pyplot as plt
import numpy as np

# Function to calculate entropy
def entropy(p):
    # Probability distribution for total number of heads
    p0 = (1 - p)**2
    p1 = 2 * p * (1 - p)
    p2 = p**2
    
    # Avoid log(0) by setting it to a small positive value
    p0 = 1e-10 if p0 == 0 else p0
    p1 = 1e-10 if p1 == 0 else p1
    p2 = 1e-10 if p2 == 0 else p2
    
    # Calculate entropy
    H = - (p0 * np.log2(p0) + p1 * np.log2(p1) + p2 * np.log2(p2))
    
    return H

# Values of p
p_values = np.linspace(0.01, 0.99, 100)

# Calculate entropy for each p
entropy_values = [entropy(p) for p in p_values]

# Plotting
plt.plot(p_values, entropy_values)
plt.title('Entropy of Total Number of Heads vs. Probability p')
plt.xlabel('p (Probability of Heads for each Coin)')
plt.ylabel('Entropy')
plt.grid(True)
plt.show()


----------------------------------------

# Task 5 - Penguin Dataset Visualization with Seaborn

## Overview

This repository contains Python code for visualizing the penguin dataset using the Seaborn library. The penguin dataset is part of the Seaborn example datasets and includes information about different penguin species, their size measurements, and environmental factors.

## Files

- **penguin_visualization.py**: Python script containing code for generating Seaborn plots to visualize various aspects of the penguin dataset.
- **penguins.csv**: CSV file containing the penguin dataset.

## Dependencies

Ensure you have the required dependencies installed. You can install them using the following:

##  ```bash
pip install seaborn matplotlib pandas

## Usage
Run the penguin_visualization.py script to generate Seaborn plots for the penguin dataset. The script loads the dataset, performs data visualization, and displays the plots.

python penguin_visualization.py

## Plots
### Pair Plot for Size Measurements:

Visualizes relationships between bill length, bill depth, flipper length, and body mass for each penguin species.

### Box Plot of Penguin Bill Length by Species:
Illustrates the distribution of bill lengths for each penguin species.

### Violin Plot of Penguin Flipper Length by Species:
Shows the distribution of flipper lengths for each penguin species.

### Scatter Plot of Penguin Bill Length vs Bill Depth:
Reveals the relationship between bill length and bill depth for individual penguins.

### Distribution Plot of Penguin Body Mass by Species:
Displays the spread of body masses for each penguin species.


# Search source
https://www.quantamagazine.org/why-mathematicians-still-cant-solve-the-collatz-conjecture-20200922/

https://www2.ifsc.usp.br/portal-ifsc/a-conjectura-de-collatz/
Explains the collatz conjecture

https://www.youtube.com/watch?v=1RL1ehEdLz4
Explains how to calculate

***********************************************************************************************************************

# Iris Dataset Analysis

## Overview

This repository contains an analysis of the well-known Iris dataset associated with Ronald A. Fisher. The dataset comprises measurements of sepal length, sepal width, petal length, and petal width for three species of iris flowers. The analysis covers variable categorization, summary statistics, and visualizations to gain insights into the dataset.

## Dataset Information

- **Source**: UCI Machine Learning Repository
- **Date Accessed**: August 17, 2023
- **URL**: [Iris Dataset](https://archive.ics.uci.edu/dataset/53/iris)

## Contents

- `project.ipynb`: Jupyter Notebook containing the Python code and analysis.
- `README.md`: This file, providing an overview of the project.

## Analysis Highlights

1. **Variable Categorization:**
   - Identified and categorized variables into numeric (interval scale) and categorical (nominal scale) types.

2. **Summary Statistics:**
   - Calculated mean, median, and standard deviation for each numeric variable.

3. **Plots:**
   - Utilized boxplots, violin plots, swarm plots, and a correlation heatmap to visualize and understand the dataset.

4. **Correlation Analysis:**
   - Explored relationships between numeric variables, revealing insights into the dataset's structure.

## Instructions

1. Clone the repository:

   ```bash
   git clone https://github.com/AnaFMello/fundamental_data_analysis_2023/blob/main/project.ipynb

2. Navigate to the project directory:
cd project


3. Open the Jupyter Notebook:
jupyter notebook project.ipynb

4. Explore the analysis, modify, or use the code for your own purposes.


## Dependencies:
Python 3
Jupyter Notebook
Required Python packages: pandas, numpy, matplotlib, seaborn

Install the dependencies using:
pip install pandas numpy matplotlib seaborn
 