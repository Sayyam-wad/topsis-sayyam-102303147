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
python topsis.py <InputDataFile> <Weights> <Impacts> <OutputResultFile>
Example:
python topsis.py data.csv "1,1,1,2" "+,+,-,+" output.csv
## Web Service (Part-III)

This repository also includes a web service implementation of the TOPSIS method as required in Part-III of the assignment.
The web service is built using Flask and allows users to perform TOPSIS analysis through a browser interface.
Features of the Web Service:
-Upload a CSV input file through a web form
-Enter weights and impacts as comma-separated values
-Provide a valid email ID
-Perform TOPSIS computation on the server
-Generate the result file containing Topsis Score and Rank
## How to Run the Web Service:
Navigate to the topsis-web folder.
Install the required dependencies using pip install -r requirements.txt.
Run the application using python app.py.
Open a browser and go to http://127.0.0.1:5000/.
This web service runs locally using Flask and demonstrates file upload, server-side processing, and result generation as part of the coursework requirements.
```bash
 

python topsis.py <InputDataFile> <Weights> <Impacts> <OutputResultFile>
