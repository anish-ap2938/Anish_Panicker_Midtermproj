# Market Basket Analysis: Frequent Itemset Mining & Association Rule Generation

This project performs Market Basket Analysis on retail transaction datasets using three different algorithms to discover frequent itemsets and generate association rules. The implemented methods include a brute force approach, an Apriori algorithm, and an FP-Growth (FP-Tree) algorithm. All algorithms are compared in terms of output consistency and execution time.

---

## Project Overview

The project is divided into four main parts:

1. **Data Creation:**  
   - Create at least 10 common retail items (e.g., diapers, clothes, electronics) and form transactions from these items.  
   - Build a transactional database with at least 20 transactions, and repeat this process to create four additional, distinct databases (totaling five datasets).  
   - **Note:** The datasets are created deterministically (either manually or sourced with proper documentation) so that the results remain reproducible.

2. **Brute Force Frequent Itemset Generation:**  
   - Enumerate all possible 1-itemsets, 2-itemsets, 3-itemsets, and so on until no further frequent itemsets are found based on a user-specified support threshold.
   - Check each itemset's frequency against the dataset.

3. **Verification with Existing Implementations:**  
   - Use an existing Apriori implementation from Python libraries to verify the results from the brute force method.
   - Use a Python package for FP-Growth to generate frequent itemsets and association rules.
   - Compare the association rules and execution times across the brute force, Apriori, and FP-Growth methods.

4. **User Interaction & Performance Evaluation:**  
   - Prompt the user once to input the minimum support and confidence thresholds.
   - Run all three algorithms on each of the five transactional datasets using these parameters.
   - Display all generated association rules and report the execution time for each algorithm.
   - Analyze whether all three algorithms produce the same results and determine which is faster under various support and confidence settings.

---

## Data

The project uses five generated CSV files representing transactions from different retail environments (e.g., Amazon, BestBuy, Kmart, Target, Walmart). Each CSV file contains at least 20 transactions with a deterministic structure to ensure reproducibility. The datasets include items typically found in supermarkets or retail stores, and the creation process is detailed in the project report.

---

## Implementation Details

- **Brute Force Method:**  
  - Enumerates all possible k-itemsets (for k = 1, 2, 3, ...) and checks their frequency.
  - Terminates when no frequent (k+1)-itemsets can be found.
  
- **Apriori Algorithm:**  
  - Uses a Python library implementation to efficiently generate frequent itemsets by leveraging the Apriori principle, which prunes the search space by eliminating infrequent itemsets early.

- **FP-Growth Algorithm:**  
  - Utilizes an FP-Tree based Python package to generate frequent itemsets without the need for candidate generation.
  
- **User-Defined Parameters:**  
  - The minimum support and confidence values are input by the user once and reused across all algorithms.
  - Multiple sets of support and confidence values are tested to demonstrate their impact on the generated association rules and performance.

- **Performance Metrics:**  
  - The output includes all discovered frequent itemsets and association rules along with their support and confidence.
  - Execution time for each algorithm is measured and compared.

---

## Output

- **Frequent Itemsets & Association Rules:**  
  - The program prints all frequent itemsets and the corresponding association rules for each dataset.
  - Each rule displays the support and confidence values.
  
- **Performance Comparison:**  
  - Execution times for the brute force, Apriori, and FP-Growth methods are reported.
  - The project analyzes whether the three algorithms yield the same results and identifies which one is faster under different parameter settings.

---

## Files Included

- `anish_panicker_midtermproj.py`: Python script for running the market basket analysis.
- `Anish_Panicker_midtermproj.ipynb`: Jupyter Notebook version of the analysis.
- `Anish_Panicker_midtermproj.pdf`: Project report documenting the implementation, results, and analysis.
- Datasets (CSV files):
  - `amazon_items.csv`
  - `bestbuy_items.csv`
  - `kmart_items.csv`
  - `target_items.csv`
  - `walmart_items.csv`

---

## License

This project is developed for educational purposes as part of a midterm assignment. All code and data are provided for academic use only.
