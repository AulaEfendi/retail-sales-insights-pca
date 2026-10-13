# Data Reduction and Big Data Using PCA on Superstore Dataset

## Project Overview
This project applies Principal Component Analysis (PCA) to the Superstore Dataset, which contains 9,994 observations and 21 variables from Kaggle. In big data, retail businesses face challenges with redundant and correlated data. PCA is used to reduce dimensionality by converting correlated variables into fewer uncorrelated principal components while retaining most information. For this analysis, 4 key numerical variables were selected: Sales, Quantity, Discount, and Profit to identify main factors influencing sales performance.

## Objectives
- To apply PCA to reduce the dimensionality from 4 variables to fewer principal components.
- To determine the number of principal components to retain using Eigenvalue Analysis and Kaiser Criterion (Eigenvalue > 1).
- To visualize PCA results using Scree Plot and Score Plot.
- To provide business implications for retail decision making.

## Tools & Technologies
- **Language:** R 4.6.0
- **IDE:** RStudio
- **Main Function:** `princomp(cor = TRUE)` using correlation matrix
- **Analysis Techniques:** Eigenvalue Analysis, Cumulative Variance, Component Loadings, Scree Plot, PCA Score Plot
- **Dataset:** Superstore Sales Dataset (Kaggle) - No missing values or duplicates

## Project Files
```
.gitignore
README.md 
project-report.pdf
r-analysis-results.txt
superstore-dataset-dashboard.xlsx
```

## Key Findings
- **Variance Explained:** PC1 = 39.75% (Eigenvalue 1.590), PC2 = 26.47% (Eigenvalue 1.059). Cumulative variance for PC1 + PC2 = 66.22%. PC3 = 22.03%, PC4 = 11.75%.
- **Component Selection:** Based on Kaiser Criterion (Eigenvalue > 1), only PC1 and PC2 are retained, reducing 4 variables to 2 components.
- **PC1 - Business Performance Component:** High loadings for Profit (0.655) and Sales (0.643), correlation with Sales r = 0.81. Represents revenue generation.
- **PC2 - Discount and Purchasing Behavior Component:** High loadings for Discount (0.719) and Quantity (0.631), correlation with Sales r = 0.22. Represents promotion strategy where higher discounts lead to higher quantity purchased.
- **Business Implication:** Managers can focus on 2 components instead of 4 variables to simplify performance analysis while retaining 66.22% of information.
