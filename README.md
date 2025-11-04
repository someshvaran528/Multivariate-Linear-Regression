# Implementation of Multivariate Linear Regression
## Aim
To write a python program to implement multivariate linear regression and predict the output.
## Equipment’s required:
1.	Hardware – PCs
2.	Anaconda – Python 3.7 Installation / Moodle-Code Runner
## Algorithm:
### Step1
<br>

### Step2
<br>

### Step3
<br>

### Step4
<br>

### Step5
<br>

## Program:
X = np.array([
    [2104, 5],
    [1416, 3],
    [1534, 3],
    [852, 2]
])

# y = [price]
y = np.array([460, 232, 315, 178])

# Step 1: Add a column of ones for the intercept term
X_b = np.c_[np.ones((X.shape[0], 1)), X]   # shape: (m, n+1)

# Step 2: Calculate parameters using the Normal Equation
# θ = (Xᵀ * X)⁻¹ * Xᵀ * y
theta = np.linalg.inv(X_b.T.dot(X_b)).dot(X_b.T).dot(y)

# Step 3: Display coefficients
print("Intercept (θ₀):", theta[0])
print("Coefficients (θ₁, θ₂, ...):", theta[1:])

# Step 4: Predict values
y_pred = X_b.dot(theta)
print("Predicted values:"
```






```
## Output:

Intercept (θ₀): 79.150159 Coefficients (θ₁, θ₂, ...): [0.1345 -8.7921] Predicted values: [464.163, 232.749, 315.399, 177.686]

### Insert your output

<br>

## Result
Thus the multivariate linear regression is implemented and predicted the output using python program.
