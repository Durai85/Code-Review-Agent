# Automated Code Review System

This project is a simple automated code review tool built using Python.  
It analyzes source code and provides quick feedback by combining **static analysis tools** with **LLM-based suggestions**.

The main idea is to reduce the amount of code sent to the LLM by **compressing context** and reviewing only meaningful parts like functions and classes.

---

## What it does

- Takes a Python source file as input  
- Breaks the code into functions and classes using AST parsing  
- Runs static analysis for:
  - Code quality
  - Style issues
  - Security warnings
- Uses an LLM to review each code block for best practices  
- Outputs clear, structured feedback  

---

## Why this project

Manual code reviews can be slow and inconsistent.  
This tool focuses on:
- Faster feedback
- Practical suggestions
- Avoiding unnecessary AI usage  

Static rules are applied first, and AI is used only where it adds value.

---

## Tech used

- Python  
- Python `ast` module  
- pylint  
- flake8  
- bandit  
- LLM API (GPT / Claude / compatible model)  

---

## How it works
Input Code <br>
↓ <br>
AST Parsing <br>
↓ <br>
Function / Class Extraction <br>
↓ <br>
Static Analysis <br>
↓ <br>
LLM Review <br>
↓ <br>
Final Report <br>
---

## Output example

- Bugs or potential errors  
- Code quality improvements  
- Best practice suggestions  

All feedback is short and actionable.

---

## Current limitations

- Supports Python only  
- Works on single files (not full repositories)  
- CLI-based interface  

---

## Future plans

- GitHub pull request integration  
- Multi-language support  
- Better feedback confidence scoring  

---

## Author

M Durai Murugan

