Overview
This project performs Market Basket Analysis using three different algorithms: Brute Force, Apriori, and FP-Growth to find frequent itemsets and generate association rules. The data consists of five transactional datasets, representing retail stores like Amazon, BestBuy, Kmart, Target, and Walmart. The project allows users to choose any dataset and analyze it based on user-defined support and confidence thresholds.

Files Included:
anish_panicker_midtermproj.py: Python script for running the market basket analysis.
Anish_Panicker_midtermproj.ipynb: Jupyter Notebook version of the analysis.
Anish_Panicker_midtermproj.pdf: Project report documenting the implementation, results, and analysis.
amazon_items.csv: Dataset containing transactions for Amazon.
bestbuy_items.csv: Dataset containing transactions for BestBuy.
kmart_items.csv: Dataset containing transactions for Kmart.
target_items.csv: Dataset containing transactions for Target.
walmart_items.csv: Dataset containing transactions for Walmart.
How to Run:
Install Required Packages: To run this project, you need to install the necessary packages:

pip install pandas mlxtend
Run the Python Script:

Open a terminal or command prompt and navigate to the directory containing the files.
Run the following command to execute the Python script:

python anish_panicker_midtermproj.py
Choose a Dataset:

After running the script, you will be prompted to choose a dataset from the five available options (Amazon, BestBuy, Kmart, Target, Walmart).
Enter a number (1-5) to select the desired dataset.
Set Support and Confidence:

The program will ask for a minimum support value (e.g., 0.2) and a minimum confidence value (e.g., 0.6).
Input the desired values, and the program will proceed with the analysis.
View Results:

The program will display frequent itemsets and association rules for the selected dataset using Brute Force, Apriori, and FP-Growth algorithms.
It will also display the time taken for each algorithm and provide a comparison of their performance.
Datasets:
Each dataset (CSV file) contains 25 transactions with 10 unique items typically found in retail stores, such as electronics, groceries, furniture, and clothes. The dataset structure includes a column labeled Items, where each row represents a transaction consisting of multiple items.

Output:
Frequent Itemsets: The program will print frequent itemsets identified by each algorithm.
Association Rules: For each frequent itemset, the program will display the association rules along with their support and confidence values.
Performance Comparison: At the end, the program compares the execution times of the three algorithms and identifies the fastest one.

License:
This project is developed for educational purposes and is part of a midterm assignment.
