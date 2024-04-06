# Apriori Recommender System

## Introduction
This project implements an Apriori recommender system using Python. Apriori is a popular algorithm for association rule mining, particularly in market basket analysis. This system analyzes transaction data to discover patterns of co-occurrence among items purchased together.

Market Basket Analysis stands as a fundamental technique employed by major retailers to unveil correlations between items. It operates by identifying combinations of items that frequently co-occur in transactions. Essentially, it enables retailers to discern relationships between the items customers purchase.

Association Rules serve as a pivotal tool for scrutinizing retail basket or transaction data, aiming to pinpoint robust rules extracted from transactional data through measures of interestingness, grounded on the principle of strong rules.

## Dataset Details
The dataset comprises 38,765 records representing purchase orders made by customers at grocery stores. These orders are amenable to analysis, and association rules can be derived using Market Basket Analysis facilitated by algorithms such as the Apriori Algorithm.

![output_8_0](https://github.com/vaishsinghds/Grocery-recommender-system/assets/161769968/961b6d48-c455-45e4-826a-5612b885667c)

## Apriori Algorithm
Apriori represents an algorithm for mining frequent itemsets and discovering association rules within relational databases. It proceeds by first identifying the frequent individual items in the database and then progressively extending them to larger item sets, contingent upon their frequent occurrence in the database. The frequent itemsets unearthed by Apriori can be harnessed to ascertain association rules, shedding light on overarching trends in the database, with practical applications spanning domains like market basket analysis.

## Illustrative Example of Association Rules
Consider a scenario with 100 customers: 10 of them purchase milk, 8 opt for butter, and 6 buy both items. The rule "bought milk => bought butter" can be assessed as follows:

Support: P(Milk & Butter) = 6/100 = 0.06
Confidence: P(Butter | Milk) = 0.06/0.08 = 0.75
Lift: Lift(Butter | Milk) = 0.75/0.10 = 7.5
It's noteworthy that this example is exceptionally small. In practical scenarios, a rule necessitates support from several hundred transactions before it attains statistical significance, and datasets typically encompass thousands or millions of transactions.

![output_17_0](https://github.com/vaishsinghds/Grocery-recommender-system/assets/161769968/98e13abc-74fa-4587-883b-45d3dea76a81)
![output_17_1](https://github.com/vaishsinghds/Grocery-recommender-system/assets/161769968/031a7b24-e387-434a-9f9d-aa502e530190)

## Key Terminology:

Support: Indicates the popularity of an itemset, quantified by the proportion of transactions where the itemset appears.
Confidence: Reflects the likelihood of item Y being purchased when item X is bought, expressed as {X -> Y}. It is measured by the proportion of transactions with item X where item Y also appears.
Lift: Gauges the likelihood of item Y being purchased when item X is bought, while accounting for the popularity of item Y.

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
- `apriori_recommender_system.ipynb`: Main Python script implementing the Apriori algorithm and generating association rules.
- `README.md`: Documentation file.

## Dataset
The system expects transaction data in CSV format with at least two columns: `Member_number` and `itemDescription`.

## Results
The system generates association rules based on the input data. These rules indicate relationships between different items purchased together, including support, confidence, lift, and other metrics.

## Acknowledgments
- This project utilizes the `mlxtend` library for implementing the Apriori algorithm.
