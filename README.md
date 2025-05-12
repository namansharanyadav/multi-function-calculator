# 🧮 Multi-Function Calculator in Python

Welcome to the **Multi-Function Calculator** built with 🐍 Python and 💻 Google Colaboratory!  
This project is a handy educational tool that performs multiple essential math operations, all from a single notebook.

## 🚀 Features

This calculator can:

🔢 **Solve proportions**  
🔍 **Solve for x** in basic algebraic equations  
🧠 **Factor square roots**  
📉 Convert **decimals** to ➡️ **fractions** and **percents**  
🍰 Convert **fractions** to ➡️ **decimals** and **percents**  
💯 Convert **percents** to ➡️ **decimals** and **fractions**

All these functions are packed in one interactive Google Colab notebook. Great for students, educators, and curious minds!

## 🛠️ Tech Stack

- 🐍 Python 3
- 📓 Google Colaboratory (Colab)

## 📂 How to Use

1. 🔗 [Open the Colab notebook](https://colab.research.google.com/drive/1Yu4r1CXczgFOEDNwVxoGXegOAUe2fHGf?usp=sharing)
2. Click **File > Save a copy in Drive** to edit your own version  
3. Follow the instructions in each cell  
4. Run the cell and input the required values  
5. 💡 See the magic happen!

## ✅ Project Goals

This challenge was built as part of a coding assignment. The aim was to reinforce Python fundamentals and learn how to build multi-functional tools efficiently.

## 🧪 Testing

The notebook includes internal tests to ensure all functions work as expected. You can try out edge cases to test the calculator's reliability.

## 📎 Example Functions

```python
# Solve proportion: a/b = c/x
def solve_proportion(a, b, c):
    return (b * c) / a

# Convert decimal to fraction
from fractions import Fraction
def decimal_to_fraction(value):
    return Fraction(value).limit_denominator()

# Factor square root
import math
def factor_square_root(n):
    outside = 1
    inside = n
    for i in range(2, int(math.sqrt(n)) + 1):
        while inside % (i * i) == 0:
            inside = inside // (i * i)
            outside *= i
    return (outside, inside)

🤝 Contributing

Pull requests are welcome! If you'd like to add more functions or improve the existing code, feel free to fork and submit a PR.
📜 License

This project is open source and free to use under the MIT License.
