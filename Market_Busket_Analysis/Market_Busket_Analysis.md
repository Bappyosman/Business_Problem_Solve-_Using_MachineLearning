# Market Basket Analysis Using Apriori Algorithm

## Project Overview

This project performs **Market Basket Analysis** using the **Apriori Algorithm** to identify frequently purchased product combinations and generate association rules from transactional data.

The analysis helps businesses understand customer purchasing patterns and supports **product recommendation, cross-selling, product bundling, and promotional strategies**.

## Objectives

* Identify frequently purchased product combinations.
* Generate association rules between products.
* Analyze Support, Confidence, and Lift.
* Discover customer purchasing patterns.
* Provide business insights for product recommendations.

## Dataset

The project uses **Market_Basket_Optimisation.csv**, a transactional dataset containing products purchased together in individual transactions.

## Methodology

1. Load the transactional dataset.
2. Clean and preprocess the data.
3. Convert transactions into a binary format.
4. Generate frequent itemsets using the Apriori Algorithm.
5. Generate association rules.
6. Evaluate rules using Support, Confidence, and Lift.
7. Extract meaningful business insights.

## Apriori Algorithm

The **Apriori Algorithm** is an association rule mining algorithm used to discover frequent itemsets in transactional data.

Example:

```text
Escalope → Pasta
```

This rule indicates that customers who purchase Escalope tend to purchase Pasta as well.

## Evaluation Metrics

### Support

Measures how frequently an itemset occurs in the entire dataset.

```text
Support(A) =
Transactions containing A
-------------------------
Total transactions
```

### Confidence

Measures the probability of purchasing B when A is purchased.

```text
Confidence(A → B) =
Support(A ∪ B)
----------------
Support(A)
```

### Lift

Measures the strength of the association between two products.

```text
Lift(A → B) =
Confidence(A → B)
------------------
Support(B)
```

| Lift | Interpretation       |
| ---- | -------------------- |
| > 1  | Positive association |
| = 1  | No association       |
| < 1  | Negative association |

## Technologies Used

* Python
* Pandas
* NumPy
* Matplotlib
* mlxtend
* Google Colab
* Apriori Algorithm

## Project Workflow

```text
Transactional Dataset
        ↓
Data Preprocessing
        ↓
Transaction Encoding
        ↓
Apriori Algorithm
        ↓
Frequent Itemsets
        ↓
Association Rules
        ↓
Support, Confidence & Lift
        ↓
Business Insights
        ↓
Product Recommendations
```

## Business Applications

### Product Recommendation

Recommend products based on the customer's current purchase or cart items.

```text
Customer adds:
Escalope

System finds:
Escalope → Pasta

Recommendation:
Pasta
```

### Cross-Selling

Businesses can recommend related products to increase the average order value.

### Product Bundling

Products that are frequently purchased together can be offered as bundles.

### Promotional Strategy

Association rules can help businesses design targeted promotions based on customer purchasing patterns.

### Store Layout Optimization

Frequently associated products can be placed closer together in physical stores.

## Example Business Interpretation

Suppose the following rule is generated:

```text
Escalope → Pasta
```

If:

```text
Support    = 0.05
Confidence = 0.30
Lift       = 1.50
```

Then:

* 5% of all transactions contain both products.
* 30% of transactions containing Escalope also contain Pasta.
* Customers who purchase Escalope are 1.5 times more likely to purchase Pasta compared with the general purchasing rate of Pasta.

## E-commerce Recommendation Logic

The association rules can be integrated into an e-commerce backend.

```text
Customer adds Product A
        ↓
Backend receives Product A
        ↓
Search association rules
        ↓
Find A → B
        ↓
Check Confidence & Lift
        ↓
Rank recommended products
        ↓
Display Product B
```

## Project Structure

```text
Market-Basket-Analysis/
│
├── dataset/
│   └── Market_Basket_Optimisation.csv
│
├── notebook/
│   └── Market_Basket_Analysis.ipynb
│
├── results/
│   └── association_rules.csv
│
├── README.md
└── requirements.txt
```

## Results

The analysis identifies frequent product combinations and association rules based on predefined support, confidence, and lift thresholds.

The generated rules can be used to identify:

* Strong product associations.
* Frequently purchased combinations.
* Potential cross-selling opportunities.
* Product recommendation opportunities.
* Potential product bundles.

## Future Improvements

* Build a real-time recommendation system.
* Integrate the model with an e-commerce backend.
* Create a recommendation API.
* Develop a business intelligence dashboard.
* Combine Apriori with other recommendation techniques.
* Update association rules using new transaction data.

## Conclusion

This project demonstrates the application of **Market Basket Analysis using the Apriori Algorithm** to discover relationships between products in transactional data.

The insights generated from association rules can support **product recommendations, cross-selling, product bundling, promotional strategies, and data-driven business decisions**.



