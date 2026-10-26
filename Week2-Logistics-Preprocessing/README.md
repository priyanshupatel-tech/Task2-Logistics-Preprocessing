# Week 2: Data Collection, Cleaning, and Preprocessing for Logistics Analysis

## Project Overview
This project demonstrates a Python-based data preprocessing pipeline for logistics analysis. It uses a sample shipment dataset to identify and handle common data quality issues before further analysis.

## Objectives
- Simulate the collection of logistics shipment data.
- Identify and handle missing numerical values.
- Detect and remove exact duplicate records.
- Detect potential outliers using the Interquartile Range (IQR) method.
- Apply IQR-based capping to extreme numerical values.
- Perform Min-Max normalization and Z-score standardization manually.
- Export the processed dataset to a CSV file.

## Tools and Libraries
- Python
- Pandas
- NumPy
- Jupyter Notebook

## Dataset Description
The sample dataset contains shipment IDs, delivery distances, delivery times, shipping costs, and delivery statuses. It intentionally includes missing values, duplicate records, and extreme numerical values to demonstrate preprocessing techniques.

## Data Preprocessing Workflow
1. Create and load the sample logistics dataset.
2. Inspect the dataset structure, missing values, duplicates, and summary statistics.
3. Fill missing numerical values using the median.
4. Remove exact duplicate rows.
5. Detect potential outliers using IQR boundaries.
6. Apply IQR-based capping to numerical outliers.
7. Perform Min-Max normalization and Z-score standardization using Pandas calculations.
8. Validate the processed data and export it to CSV.

## Project Files
- `week2_logistics_preprocessing.ipynb` — Jupyter Notebook containing the implementation.
- `logistics_data.csv` — Original sample dataset.
- `logistics_preprocessed.csv` — Processed dataset containing cleaned data and transformed numerical columns.

## How to Run
1. Install Python and Jupyter Notebook.
2. Install the required libraries:
   `pip install pandas numpy matplotlib`
3. Open `week2_logistics_preprocessing.ipynb` in Jupyter Notebook.
4. Run the notebook cells in sequence.

## Normalization Methods
Min-Max normalization transforms numerical values to a range between 0 and 1 when the column has varying values.

Z-score standardization transforms values based on the column mean and standard deviation.

Both methods are implemented manually without using `MinMaxScaler` or `StandardScaler`.

## Conclusion
This project demonstrates how data quality affects logistics analytics. Handling missing values, duplicates, and extreme observations can improve the reliability of downstream analysis. The resulting processed dataset is prepared for further exploration and analytical tasks.

## Note
The dataset is simulated for educational purposes and is not a record of actual logistics operations. Outlier capping is a preprocessing choice and should be validated against domain knowledge in real-world applications.
