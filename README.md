# topsis-sayyam-102303147

## TOPSIS Implementation in Python(Part-I)

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

## Usage(Part-2)
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
# Methodology
The TOPSIS (Technique for Order Preference by Similarity to Ideal Solution) method is a multi-criteria decision-making approach used to rank alternatives based on their closeness to an ideal solution.
The methodology followed in this project is outlined below:
1. **Decision Matrix Formation**
   The input CSV file forms the decision matrix. Each row represents an alternative, and each column (except the first) represents a criterion.
2. **Normalization**
   The decision matrix is normalized using vector normalization to remove scale differences among criteria.
3. **Weight Application**
   User-defined weights are applied to the normalized values to reflect the relative importance of each criterion.
4. **Ideal Best and Ideal Worst**
   Based on impacts provided:
* For positive (+) impact criteria, the maximum value is considered ideal best.
* For negative (-) impact criteria, the minimum value is considered ideal best.
5. **Distance Measures**
   Euclidean distances of each alternative from the ideal best and ideal worst solutions are calculated.
6. **TOPSIS Score and Ranking**
   The TOPSIS score is computed as the relative closeness to the ideal solution. Alternatives are ranked in descending order of these scores.
# Result Table
The output CSV file contains the original data along with two additional columns:
* **Topsis Score**: Indicates the relative performance of each alternative.
* **Rank**: Represents the final ranking (Rank 1 being the best alternative).
This table provides a clear comparison of alternatives based on the selected criteria, weights, and impacts.
# Result Interpretation
An alternative with a higher TOPSIS score is considered closer to the ideal solution and therefore ranks higher. The final ranking is influenced by the dataset values, assigned weights, and impact directions.
# Conclusion
This TOPSIS implementation offers a systematic and reproducible solution for multi-criteria decision making. By allowing flexible weights and impacts, it enables objective comparison of alternatives and supports informed decision-making across different scenarios.
