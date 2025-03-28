# DataStructer_-Infix-to-Postfix-Conversion-and-Evaluation-Using-Expression-Trees-in-C
# 📐 Infix to Postfix Conversion and Evaluation Using Expression Trees in C

### 👤 Author: Mariam Turk  
**Student ID:** 1211115  
**Section:** 1  
**Instructor:** Ahmad Abusnaina  

---

## 🧠 Overview

This C program provides a complete system for processing mathematical expressions:

- ✅ Converts **infix expressions** to **postfix notation**
- 🌳 Builds **expression trees** from postfix expressions
- 🧮 Evaluates expressions using tree-based traversal
- 💾 Supports file I/O for loading and saving expressions

---

## 🔧 Features

- 🗂 Load multiple infix expressions from a file
- 📝 Clean expressions from whitespace and special characters
- ➕ Convert to **postfix notation**
- 🧠 Evaluate using **expression tree**
- 📄 Save postfix expressions and results to a file
- 📋 Menu-driven user interface

---

## 📁 File Structure

. ├── main.c # C source code ├── input.txt # File containing infix expressions (one per line) ├── output.txt # File to store postfix and evaluation results └── README.md # Project documentation

yaml
Copy
Edit

---

## 🧪 Sample Input (`input.txt`)

(3 + 5) * 2 10 + 4 * 3 100 / (5 + 5)

yaml
Copy
Edit

---

## 📤 Sample Output (`output.txt`)

Postfix expression for '(3 + 5) * 2': 3 5 + 2 * Result: 16

Postfix expression for '10 + 4 * 3': 10 4 3 * + Result: 22

Postfix expression for '100 / (5 + 5)': 100 5 5 + / Result: 10

yaml
Copy
Edit

---

## 🚀 How to Run

### ✅ Compile the Code
```bash
gcc main.c -o expr_tree
▶️ Run the Program
bash
Copy
Edit
./expr_tree
🧭 Menu Options
mathematica
Copy
Edit
1. Read equations
2. Print equations
3. Evaluate using Expression tree
4. Print postfix expressions
5. Save to output file (postfix and results)
6. Exit
🔍 Key Data Structures
Structure	Role
Stack	Used in infix-to-postfix conversion
Expression Tree	Used for evaluation of expressions
Doubly Linked List	Used to store multiple expressions
⚙️ Core Functionalities
clearWS_SC() – Sanitizes input expressions

preConverter() – Converts infix to postfix

stack_ET() – Builds expression tree from postfix

calu_tree() – Recursively evaluates expression tree

loadFromFile() – Loads expressions from input.txt

fprintf() – Saves results to output.txt
