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



---

### Model validation

The notebooks include:
- Visualization of gradient descent convergence
- Comparison of predictions vs actual values
- Analysis of different learning rates
- Cost surface visualization

### AWS SageMaker

#### Process
- Create AWS Sagemaker Studio
- Create a new Notebook enviroment
- Upload both jupyter notebooks
- Select respective kernel and run all cells

#### Evidence 

Sagemaker domain
![imagen](/public/prueba4.png)

Select a profile and go to studio
![imagen](/public/prueba5.png)

Rund and open the code builer space
![imagen](/public/prueba6.png)

Open or create the folder where the notebooks will be 
![imagen](/public/prueba7.png)

![imagen](/public/prueba8.png)

Select Kernel
![imagen](/public/prueba9.png)

Run all cells
![imagen](/public/prueba1.png)
![imagen](/public/prueba2.png)
![imagen](/public/prueba3.png)


Note: No differences were observed between local and cloud execution 


# Key Concepts

### Cost Function

Used to determine how badly a model is predicting.

$$
\text{MSE} = \frac{1}{n} \sum_{i=1}^{n} (y_i - \hat{y}_i)^2
$$


Where:
  - $y$ = Value
  - $\hat{y}$ = Predicted value
  -  $n$ = Number of data
---
### Cost Surface 

Shows how good or bad the model is for each possible combination of parameters.

---

### Gradient

Its vector of partial derivatives that indicates the direction and rate of greatest increase of a function

The negative gradient is used to minimize the cost function.

---

### Gradient Descent
Optimization algorithm to find the parameters that minimize the cost function

$$
w := w - \alpha \frac{\partial J}{\partial w}, \qquad
b := b - \alpha \frac{\partial J}{\partial b}
$$

---

### Vectorization

Replace explicit loops with vector operations to make calculations faster and more efficient.

### Stellar luminosity as a function

$$
\hat{L} = wM+b
$$


---


# Datasets


### Part 1

```
M = [0.6, 0.8, 1.0, 1.2, 1.4, 1.6, 1.8, 2.0, 2.2, 2.4]
L = [0.15, 0.35, 1.00, 2.30, 4.10, 7.00, 11.2, 17.5, 25.0, 35.0]
```

Where
 - **M**: Stellar mass
 - **L**: Luminosity  

### Part 2

```
M = [0.6, 0.8, 1.0, 1.2, 1.4, 1.6, 1.8, 2.0, 2.2, 2.4]
T = [3800, 4400, 5800, 6400, 6900, 7400, 7900, 8300, 8800, 9200]
L = [0.15, 0.35, 1.00, 2.30, 4.10, 7.00, 11.2, 17.5, 25.0, 35.0]
```

Where
 - **M**: Stellar mass
 - **L**: Luminosity 
 - **T**: Temperature 



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
