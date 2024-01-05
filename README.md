# fundamental_data_analysis_2023
## Ana Mello

***********************************************************************************************************************

# Iris Dataset Analysis

## Overview
This Jupyter Notebook, named tasks.ipynb, encompasses five distinct tasks, each addressing different aspects of data analysis, probability distributions, and visualization. This README provides a guide on how to understand and run each task individually, along with prerequisites and considerations for seamless execution.

## Prerequisites
Before proceeding, make sure you have the required Python libraries installed. You can install them using the following:

pip install numpy pandas seaborn matplotlib

Ensure that you have Jupyter Notebook installed to run the tasks interactively. If not, you can install it using:
pip install jupyter

## Task 1: Collatz Conjecture Verification
Usage:

Open tasks.ipynb in your Jupyter Notebook environment.

Execute the cells containing the collatz_sequence and verify_collatz_conjecture functions.

Run the cell that calls verify_collatz_conjecture(10000) to verify the Collatz conjecture for the first 10,000 positive integers.

## Task 2: Penguins Dataset Overview and Variable Modeling
Usage:

Open tasks.ipynb in your Jupyter Notebook environment.

Execute the cell loading the penguins dataset using pd.read_csv.

Run the cells generating dataset overviews, summary statistics, and variable modeling.

Explore the pairplot visualization to understand relationships between numeric variables.

## Task 3: Probability Distribution Modeling for Penguins Dataset Variables
Usage:

Open tasks.ipynb in your Jupyter Notebook environment.

Execute the cell loading the penguins dataset using pd.read_csv.

Run the cells defining the entropy function and calculating entropy values for different combinations of probabilities.

Visualize the entropy heatmap to observe changes with varying probabilities.

## Task 4: Entropy of Two Coin Flips
Usage:

Open tasks.ipynb in your Jupyter Notebook environment.

Execute the cell defining the entropy function.

Run the cell generating entropy values for different probabilities.

Visualize the entropy heatmap to observe changes in entropy for varying probabilities.

## Task 5: Individual Plots for Penguin Dataset Variables
Usage:

Open tasks.ipynb in your Jupyter Notebook environment.

Execute the cell loading the penguins dataset using sns.load_dataset.

Run the individual cells for each plot (pairplot, box plot, violin plot, scatter plot, and distribution plot).

Explore each plot's insights into the penguins dataset variables.

# Search source

Task 1: Collatz Conjecture Verification

Wikipedia - Collatz Conjecture: https://en.wikipedia.org/wiki/Collatz_conjecture

MathWorld - Collatz Problem: https://mathworld.wolfram.com/CollatzProblem.html

Mathematics Stack Exchange - Collatz Conjecture: https://math.stackexchange.com/questions/tagged/collatz-conjecture

Task 2: Penguins Dataset Overview and Variable Modeling

Seaborn Documentation - Datasets: https://seaborn.pydata.org/introduction/plotting_distributions.html#plotting-distributions-tutorial

Pandas Documentation - Reading CSV Files: https://pandas.pydata.org/docs/reference/api/pandas.read_csv.html

Towards Data Science - Exploratory Data Analysis with Seaborn: https://towardsdatascience.com/exploratory-data-analysis-with-seaborn-508a5e8180c3

Task 3: Probability Distribution Modeling for Penguins Dataset Variables

NumPy Documentation - Random Sampling: https://numpy.org/doc/stable/reference/random/index.html

SciPy Documentation - Continuous Distributions: https://docs.scipy.org/doc/scipy/reference/stats.html#continuous-distributions

Kaggle Notebook - Understanding Probability Distributions: https://www.kaggle.com/prasadperera/theoretical-distributions

Task 4: Entropy of Two Coin Flips

Wolfram MathWorld - Entropy: https://mathworld.wolfram.com/Entropy.html

Stack Exchange - Cross Validated: https://stats.stackexchange.com/

Information Theory - Shannon's Entropy: https://www.informationtheory.org/

Task 5: Individual Plots for Penguin Dataset Variables

Seaborn Documentation - Pairplot: https://seaborn.pydata.org/generated/seaborn.pairplot.html

Seaborn Documentation - Boxplot: https://seaborn.pydata.org/generated/seaborn.boxplot.html

Seaborn Documentation - Violinplot: https://seaborn.pydata.org/generated/seaborn.violinplot.html

Seaborn Documentation - Scatterplot: https://seaborn.pydata.org/generated/seaborn.scatterplot.html

Seaborn Documentation - Histplot: https://seaborn.pydata.org/generated/seaborn.histplot.html

Matplotlib Documentation: https://matplotlib.org/stable/contents.html

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
 