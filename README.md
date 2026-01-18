# topsis-sayyam-102303147

## TOPSIS Implementation in Python

This repository contains a Python implementation of the **TOPSIS (Technique for Order Preference by Similarity to Ideal Solution)** method for multi-criteria decision making.

The project provides a command-line interface (CLI) to evaluate and rank alternatives based on weighted criteria and their positive or negative impacts. It is suitable for academic use as well as basic real-world decision analysis tasks.

---

## What is TOPSIS?

TOPSIS is a multi-criteria decision-making technique that ranks alternatives based on their relative closeness to the ideal best and ideal worst solutions.

An alternative with the **highest TOPSIS score** is considered the best choice.

---

## Features

- Command-line based implementation  
- Accepts CSV input files  
- Supports user-defined weights and impacts  
- Generates TOPSIS score and rank for each alternative  
- Robust input validation and error handling  
- Simple and reproducible workflow  

---
## User Manual

### Installation

pip install topsis-sayyam-102303147

## Usage

### Command Format
```bash
 

python topsis.py <InputDataFile> <Weights> <Impacts> <OutputResultFile>
