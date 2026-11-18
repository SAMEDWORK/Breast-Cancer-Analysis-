## Project Summary
This project analyzes the Breast Cancer Wisconsin (Diagnostic) dataset: 569 tumor cases with cell-nucleus measurements, labeled malignant or benign. It uses Python, Pandas, NumPy, Matplotlib, and Seaborn for dataset exploration, data cleaning, feature engineering, visualization, and insight generation, with the results documented in a written report.

**Data note:** the original dataset is already clean, so a few missing values, inconsistent labels, and duplicate rows were deliberately introduced and then cleaned to demonstrate the cleaning workflow.

## Key Findings
- **Class balance:** 357 benign (62.7%) and 212 malignant (37.3%) cases.
- **Cleaning:** 5 duplicate rows removed, 37 missing values filled with column medians, and inconsistent diagnosis labels standardized.
- **Size is the strongest signal:** perimeter, radius, and area correlate most strongly with diagnosis (r ≈ -0.74, -0.73, -0.71 with benign coded as 1).
- **Malignant tumors are larger:** average radius is about 17.5 vs 12.2 for benign, and average area is about 978 vs 463.
- **Malignancy rate rises with size:** from 3.5% in the smallest tumor category to 100% in the largest.
- **Shape adds a secondary signal:** concavity and compactness are higher in malignant cases.

**Conclusion:** tumor size (radius, perimeter, area) is the most reliable predictor of malignancy in this dataset, with shape irregularity as a useful supporting feature.
