## TOPSIS Python Package

### **Description**

This program is an extension of Program 1 and provides the same TOPSIS functionality as an installable Python package. It allows users to use the TOPSIS method programmatically in their projects or via the command line.

### **Features**

- Installable Python package.
- Usable via both Python code and CLI.
- Validates inputs and provides meaningful error messages.

### **Installation**

Install the package using pip:

```bash
pip install Topsis-Nitin-102203984
```

### **Usage**

#### **Command Line**

```bash
topsis-cli <input_file> <weights> <impacts> <output_file>
```

Example:

```bash
topsis-cli data.csv "1,2,3,4" "+,-,+,-" result.csv
```

#### **Python Code**

```python
from Topsis_Nitin_102203984 import topsis

# Example usage
topsis("data.csv", "1,2,3,4", "+,-,+,-", "result.csv")
```

### **Dependencies**

- Python 3.x
- pandas
- numpy

### **Files to Upload to PyPI**

- `setup.py`
- `README.md`
- `LICENSE.txt`
- The module directory (e.g., `Topsis_Nitin_102203984/`)

### **Development**

To build and distribute the package:

1. Build the package:
   ```bash
   python setup.py sdist bdist_wheel
   ```
2. Upload to PyPI:
   ```bash
   twine upload dist/*
   ```

### **Limitations**

- The package does not handle non-numeric data in criteria columns.
- Ensure that weights and impacts are provided in the correct format.

---
