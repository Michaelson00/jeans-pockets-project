# Jean Pockets Project
<pre>
jean-pockets-project
│
├── data
│   └── jean-pocket-measurements.csv
│
├── notebooks
│   └── jean-pockets-analysis.ipynb
│
├── images
│   ├── pocket-height-style-gender.png
│   └── phone-fit-percentage.png
│
└── README.md
</pre>

# Project Overview
This project analyses jean pocket measurements to investigate a common question:
Are women’s jean pockets actually smaller than men’s?
Using Python and data analysis tools, pocket measurements from different jean brands and <br>
styles were explored to compare pocket sizes between genders and determine whether modern smartphones can fit inside them.

# Tools used
- Python
- Pandas
- Matplotlib / Seaborn
- SciPy (statistical testing)
- Jupyter Notebook

# Research Questions
## 1. What is the average difference in pocket height_front between women's and men's jeans?
The analysis shows a large difference in front pocket depth between genders.
Average front pocket height (women): 14.33 cm
Average front pocket height (men): 23.13 cm
Average difference:
Men’s front pockets are approximately 8.80 cm deeper than women’s on average.

## 2. Is there a significant difference in pocket height_front between skinny and straight styles within the same gender?
Independent t-tests were conducted to compare skinny and straight styles.
Results:
Women: p-value ≈ 0.865
Men: p-value ≈ 0.868
Since both p-values are greater than 0.05, there is no statistically significant difference in front pocket height between skinny and straight styles within the same gender.
This suggests pocket depth differences are primarily driven by gender rather than style.

## 3. How do back pocket sizes compare between women's and men's jeans?
Back pocket size was compared by calculating pocket area:
Back Pocket Area = height_back × width_back
Average back pocket area:
Women: 201.82 cm²
Men: 219.71 cm²
Men’s back pockets are slightly larger on average, but the difference is much smaller compared to the front pocket depth difference.

## 4. What percentage of women's and men's jeans can fit an iPhone 12?
The iPhone 12 height is approximately 14.7 cm.
A pocket was considered able to fit the phone if:
height_front ≥ 14.7 cm
Results:
Men's jeans: 100% can fit the phone
Women's jeans: 30% can fit the phone

This highlights a major practical difference: most women's front pockets are too shallow to fit a modern smartphone.

# Conclusion
The analysis supports the widely discussed claim that women’s jean pockets are significantly smaller than men’s, particularly in front pocket depth.

# Key findings:
- Men’s front pockets are ~8.8 cm deeper on average
- Style differences (skinny vs straight) do not significantly affect pocket depth
- Back pocket sizes differ slightly but not dramatically
- Only 30% of women's jeans can fit an iPhone 12, compared to 100% of men's
