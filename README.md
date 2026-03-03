The dataset was loaded and the first five rows were displayed to confirm that it was read correctly. The shape was checked to understand the number of rows and columns, which confirmed the dataset structure.

Data types were inspected using the information summary. The columns sex and smoker were converted from object to category because they represent categorical variables. This improves clarity and reduces memory usage.

Missing values were checked, and none were found. However, a general strategy was prepared: numerical values would be filled with the median and categorical values with the mode if needed. This ensures robustness and reusability.

Duplicate rows were checked and one duplicate was removed to prevent bias in analysis.

Outliers were examined in the target variable charges. Extreme values above the 99th percentile were capped instead of removed to reduce their impact while keeping all observations.

All steps were combined into a reusable cleaning function. Finally, validation checks confirmed that there are no missing values, all target values are positive, and the dataset structure remains correct.
