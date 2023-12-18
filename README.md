# Survival Prediction
## Leslie Matrix Population Projection
This Mathematica code performs population projection using the Leslie Matrix, a common tool in population biology and demography. The Leslie Matrix is used to model population growth based on age-specific fertility rates and survival rates.

## Leslie Matrix Definition
```
L = {{0.000, 0.045, 0.391, 0.472, 0.484, 0.546, 0.543, 0.502, 0.468, 0.459, 0.433, 0.421},
     {0.845, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0},
     {0, 0.975, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0},
     {0, 0, 0.965, 0, 0, 0, 0, 0, 0, 0, 0, 0},
     {0, 0, 0, 0.950, 0, 0, 0, 0, 0, 0, 0, 0},
     {0, 0, 0, 0, 0.926, 0, 0, 0, 0, 0, 0, 0},
     {0, 0, 0, 0, 0, 0.895, 0, 0, 0, 0, 0, 0},
     {0, 0, 0, 0, 0, 0, 0.850, 0, 0, 0, 0, 0},
     {0, 0, 0, 0, 0, 0, 0, 0.786, 0, 0, 0, 0},
     {0, 0, 0, 0, 0, 0, 0, 0, 0.691, 0, 0, 0},
     {0, 0, 0, 0, 0, 0, 0, 0, 0, 0.561, 0, 0},
     {0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0.370, 0}}; (* Leslie Matrix *)
```
## Eigensystem Analysis
The code computes the eigenvalues and eigenvectors of the Leslie Matrix.

## Population Projection
We initialize an initial population vector (```xVec```) and computes the next population using matrix-vector multiplication (```L.xVec```). The recursive method is repeated for a specified number of iterations (n). The results are stored in the ```results``` list, and the population evolution over time is displayed in a matrix format.

## Population Visualization
The code further visualizes the population projection over multiple years, providing a line plot for each age group. The x-axis represents the years, and the y-axis represents the population for each age group.

## Usage
Copy and paste the code into a Mathematica notebook.
Evaluate the code to perform Leslie Matrix population projection and visualize the results.

## Note
Adjust the initial population (```initPop```) and the number of iterations (```endNum```) based on specific requirements. The code provides a flexible framework for exploring different scenarios and understanding the impact on population dynamics.
