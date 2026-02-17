# Dataset Information

## About the Dataset

This project uses the **Bank Marketing Dataset** from the UCI Machine Learning Repository.

**Dataset**: Bank Marketing Data Set  
**Source**: [UCI Machine Learning Repository](https://archive.ics.uci.edu/ml/datasets/Bank+Marketing)

## How to Obtain the Data

Due to copyright considerations, the dataset is not included in this repository. Please follow these steps to obtain it:

1. Visit the [UCI Machine Learning Repository - Bank Marketing Dataset](https://archive.ics.uci.edu/ml/datasets/Bank+Marketing)

2. Download the **bank-full.csv** file (the complete dataset with all examples)

3. Place the downloaded file in this `data/` directory

4. Your directory structure should look like:
   ```
   data/
   ├── README.md (this file)
   └── bank-full.csv (the downloaded dataset)
   ```

## Dataset Description

The data is related to direct marketing campaigns (phone calls) of a Portuguese banking institution. The marketing campaigns were based on phone calls. Often, more than one contact to the same client was required in order to assess if the product (bank term deposit) would be ('yes') or not ('no') subscribed.

### File Information
- **File**: bank-full.csv
- **Format**: CSV with semicolon (;) delimiter
- **Size**: ~4,500 KB
- **Instances**: 45,211
- **Features**: 17 (16 input features + 1 output variable)

### Features

**Bank client data:**
1. age (numeric)
2. job (categorical)
3. marital (categorical)
4. education (categorical)
5. default (categorical)
6. balance (numeric)
7. housing (categorical)
8. loan (categorical)

**Related to the last contact of the current campaign:**
9. contact (categorical)
10. day (numeric)
11. month (categorical)
12. duration (numeric)

**Other attributes:**
13. campaign (numeric)
14. pdays (numeric)
15. previous (numeric)
16. poutcome (categorical)

**Output variable (target):**
17. y - has the client subscribed to a term deposit? (binary: 'yes','no')

## Citation

If you use this dataset in your own work, please cite:

```
[Moro et al., 2014] S. Moro, P. Cortez and P. Rita. 
A Data-Driven Approach to Predict the Success of Bank Telemarketing. 
Decision Support Systems, Elsevier, 62:22-31, June 2014
```

## License

The dataset is publicly available from the UCI Machine Learning Repository for research and educational purposes.
