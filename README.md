# README

## Overview
This script demonstrates two tasks using NumPy in Python:
1. **Replicating NumPy Broadcasting Using For Loops** – This task manually replicates NumPy's broadcasting feature by performing element-wise division using nested for loops.
2. **Converting a Python Dictionary to a NumPy Array** – This task converts a dictionary containing lists into a NumPy array and presents the data in a structured format.

## Requirements
To run this script, ensure you have Python installed along with the required library:

```sh
pip install numpy
```

## Usage
Run the script using Python:
```sh
python script.py
```

## Task 1: Replicating Broadcasting Using For Loops
- Generates random 4×4 and 1×4 NumPy arrays.
- Performs element-wise division using NumPy's broadcasting.
- Implements a manual version using nested for loops.
- Verifies that both methods yield identical results.

### Expected Output:
```
Result using broadcasting:
[[-0.49214189  0.45607819  0.28183596 -3.90043439]
 [-0.26229311  0.75518888 -2.41688145 -1.11063629]
 [ 0.57387869 -0.39635354 -0.67614513 -0.2452416 ]
 [ 0.676082   -0.29216483 -0.44218937 -1.12471925]]

Result using for loops:
[[-0.49214189  0.45607819  0.28183596 -3.90043439]
 [-0.26229311  0.75518888 -2.41688145 -1.11063629]
 [ 0.57387869 -0.39635354 -0.67614513 -0.2452416 ]
 [ 0.676082   -0.29216483 -0.44218937 -1.12471925]]

Results match!
```

## Task 2: Converting a Dictionary to a NumPy Array
- Defines a dictionary with keys `Name`, `Age`, and `Score`.
- Converts dictionary values into a NumPy array.
- Prints the original dictionary and the transformed array.
- Optionally transposes the array for better readability.

### Expected Output:
```
Dictionary:
{'Name': ['Ed', 'Edd', 'Eddie'], 'Age': [25, 30, 35], 'Score': [85.5, 90.0, 88.0]}

Converted NumPy array:
[['Ed' 'Edd' 'Eddie']
 ['25' '30' '35']
 ['85.5' '90.0' '88.0']]

Transposed NumPy array:
[['Ed' '25' '85.5']
 ['Edd' '30' '90.0']
 ['Eddie' '35' '88.0']]
```

## Notes
- The script sets a random seed for reproducibility.
- `assert np.allclose(A_broadcast, A_loop)` ensures the manually computed values match NumPy’s broadcasting.
- The dictionary-to-array conversion assumes uniform-length lists.

## Author
Developed by Jeremy Martinez-Quinones.

## License
This project is licensed under the MIT License - see LICENSE file for details.
