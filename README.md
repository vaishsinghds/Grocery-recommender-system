# Apriori Recommender System

## Introduction
This project implements an Apriori recommender system using Python. Apriori is a popular algorithm for association rule mining, particularly in market basket analysis. This system analyzes transaction data to discover patterns of co-occurrence among items purchased together.

## Requirements
- Python 3.x
- pandas
- mlxtend

## Installation
You can install the required libraries using pip:
pip install pandas mlxtend


## Usage
1. Clone the repository or download the project files.
2. Ensure that your transaction data is in a suitable format. In this project, the data is assumed to be in CSV format.
3. Update the file path in the code to point to your dataset.
4. Run the `apriori_recommender_system.ipynb` script.

## Files
- `apriori_recommender.py`: Main Python script implementing the Apriori algorithm and generating association rules.
- `README.md`: Documentation file.
- `LICENSE`: License information.

## Dataset
The system expects transaction data in CSV format with at least two columns: `Member_number` and `itemDescription`.

## Results
The system generates association rules based on the input data. These rules indicate relationships between different items purchased together, including support, confidence, lift, and other metrics.

## Acknowledgments
- This project utilizes the `mlxtend` library for implementing the Apriori algorithm.
