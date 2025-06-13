# Quantum S Gate Demonstration

This notebook demonstrates the effect of the **S gate** (also called the **Phase gate**) on six fundamental quantum states:  
**|0⟩**, **|1⟩**, **|+⟩**, **|−⟩**, **|i⟩**, and **|−i⟩**.

The S gate performs a **π/2 (90°) phase rotation** around the Z-axis on the Bloch sphere.  
It introduces a complex phase factor of *i* to the |1⟩ state while keeping the |0⟩ state unchanged.

---

## 🔧 Gate Definition

The S gate is represented by the following unitary matrix:

```

S = [[1, 0],
    [0, i]]

````

---

## 🧠 States Tested

The following six quantum states are tested:

| Name   | Symbol | Vector Form                                       |
|--------|--------|---------------------------------------------------|
| Zero   | \|0⟩    | [1, 0]                                            |
| One    | \|1⟩    | [0, 1]                                            |
| Plus   | \|+⟩    | (1/√2) × [1, 1]                                   |
| Minus  | \|−⟩    | (1/√2) × [1, −1]                                  |
| i      | \|i⟩    | (1/√2) × [1, i]                                   |
| −i     | \|−i⟩   | (1/√2) × [1, −i]                                  |

---

## 🎯 Results After Applying S Gate

| Input  | Output     |
|--------|------------|
| \|0⟩   | \|0⟩       |
| \|1⟩   | *i*\|1⟩     |
| \|+⟩   | (1/√2)[1, *i*] = \|i⟩ |
| \|−⟩   | (1/√2)[1, −*i*] = \|−i⟩ |
| \|i⟩   | Becomes complex rotation |
| \|−i⟩  | Becomes complex rotation |

🧾 Note: The S gate **adds a phase of π/2 to |1⟩**, transforming superpositions by twisting them in the complex plane.

---

## 📓 Notebook Contents

- Definition of the S gate using NumPy
- Construction of 6 input quantum states
- Matrix multiplication to apply the gate
- Output display of resulting states with explanation

---

## ▶️ How to Run

1. Make sure Python is installed
2. Install NumPy if not already:
```bash
pip install numpy
````

3. Open and run:

```bash
jupyter notebook Sgate.ipynb
```

---

## 📚 Learning Outcome

The S gate is fundamental in phase-based quantum operations.
Understanding its effect prepares you for algorithms involving **quantum Fourier transforms, phase estimation**, and **quantum cryptography**.

---
