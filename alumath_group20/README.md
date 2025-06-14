alumath_group20 :
A Python library for matrix operations, supporting multiplication of matrices with different dimensions, developed by Group 20: Christian, Carine, Eva, and Thierry.

View it at: https://pypi.org/project/alumath-group20/0.1.0/

Installation

Install via pip:
pip install alumath_group20

Usage
The alumath_group20 library, created by Christian, Carine, Eva, and Thierry, provides a Matrix class for matrix multiplication with compatible dimensions. 

Below are examples:
Example 1: Multiplying Two 2x2 Matrices

from alumath_group20 import Matrix

# Define two 2x2 matrices
A = Matrix([[1, 2], [3, 4]])
B = Matrix([[5, 6], [7, 8]])

# Multiply using @
C = A @ B
print("2x2 * 2x2 Matrix:")
print(C)

Output:
2x2 * 2x2 Matrix:
19 22
43 50

Example 2: Multiplying a 2x3 Matrix by a 3x2 Matrix
from alumath_group20 import Matrix

# Define a 2x3 and a 3x2 matrix
X = Matrix([[1, 2, 3], [4, 5, 6]])
Y = Matrix([[7, 8], [9, 10], [11, 12]])

# Multiply
Z = X @ Y
print("2x3 * 3x2 Matrix:")
print(Z)

Output:
2x3 * 3x2 Matrix:
58 64
139 154

Example 3: Handling Incompatible Dimensions
from alumath_group20 import Matrix

# Define incompatible matrices (1x2 and 3x1)
A = Matrix([[1, 2]])
B = Matrix([[1], [2], [3]])

try:
    C = A @ B
except ValueError as e:
    print(e)

Output (member name varies):
Matrix dimensions incompatible for multiplication, says Christian, Carine, Eva, or Thierry(name is picked randomly)

Notes :

Supports multiplication for compatible dimensions (m×n * n×p = m×p).
For incompatible dimensions, raises ValueError with a message including a randomly selected member (Christian, Carine, Eva, or Thierry).
Uses the @ operator for multiplication.

Development
To contribute:

Clone the repository:
git clone https://github.com/yourusername/alumath_group20.git
cd alumath_group20


Install in editable mode:
pip install -e .


Run tests:
python -m unittest tests/test_matrix.py



License
MIT License


Authors :

Christian
Carine
Eva
Thierry
