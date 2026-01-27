# Linear and Polynomial Models for Regression

This project implements linear and polynomial regression models from scratch to model the stellar mass-luminosity relationship. The lab is divided into two parts: the first implements simple linear regression with one feature (stellar mass), and the second extends the model to polynomial regression with multiple features (mass and temperature). Gradient descent algorithms are implemented in both vectorized and non-vectorized versions, the cost surface is visualized, and different models and learning rates are compared.

## Getting Started

These instructions will get you a copy of the project up and running on your local machine for development and testing purposes. See deployment for notes on how to deploy the project on a live system.

### Prerequisites

- Python 3.3 or higher
- Jupyter Notebook or JupyterLab
- Python libraries:
  - numpy
  - matplotlib
  - mpl_toolkits (included with matplotlib)

Example of dependency installation:
```bash
pip install numpy matplotlib
```

### Installing

Steps to set up the development environment:

1. Clone or download the project repository

2. Install the necessary dependencies:
```bash
pip install numpy matplotlib
```

3. Open the notebooks in Jupyter:
```bash
jupyter notebook
```

4. Run the notebooks in order:
   - `01_part1_linreg_1feature.ipynb`: Simple linear regression
   - `02_part2_polyreg.ipynb`: Polynomial regression with multiple features



## Running the tests

This project does not include automated tests, but the notebooks contain validations and visualizations that allow verifying the correct operation of the models:

### Model validation

The notebooks include:
- Visualization of gradient descent convergence
- Comparison of predictions vs actual values
- Analysis of different learning rates
- Cost surface visualization





## Built With

* [NumPy](https://numpy.org/) - Numerical computation and array operations
* [Matplotlib](https://matplotlib.org/) - Data visualization and plotting
* [Jupyter Notebook](https://jupyter.org/) - Interactive development environment
* [Python](https://www.python.org/) - Programming language



## Authors

* **Santiago Suarez** - *Lab work* - TDSE Lab 1

This project was developed as part of the linear and polynomial regression lab.



## Acknowledgments

* Example data based on the stellar mass-luminosity relationship from astrophysics
* Machine learning concepts and linear regression
* Educational implementation of gradient descent from scratch
