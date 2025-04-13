# Leaf Classification with Principal Component Analysis (PCA)

![Leaves](https://external-content.duckduckgo.com/iu/?u=https%3A%2F%2Fmiro.medium.com%2Fmax%2F942%2F1*vMJbpi6Lj9kkvNV5HnrcqA.jpeg&f=1&nofb=1&ipt=8485e6c0ac778a84d6a16aa076377b780134acbfcecf5d846fe9fcead56265e7)

## Project Overview
This project is part of a university practical assignment (TP) focused on the **study and classification of tree leaves** using a set of predefined descriptors. The main goal was to explore the dataset through dimensionality reduction and assess the potential of various classification techniques inspired by methods studied in class.

## Dataset

I chose to work on the dataset provided in the TP, which consists of a collection of leaf images, each described by several morphological and statistical descriptors such as:

- Solidity
- Eccentricity
- Aspect Ratio
- Roundness
- Moments
- Convexity
- etc.

These descriptors were used as input features for the analysis. The corresponding images are found in the `Leaf images` folder, but the main focus was on their associated numerical representations.

## Objective

The objective of the project was to:
- Understand and explore the structure of the data.
- Apply dimensionality reduction techniques like **ACP (Analyse en Composantes Principales / PCA)**.
- Visualize and interpret the data in the reduced space.
- Optionally apply classification techniques such as logistic regression or clustering (KMeans, etc.).

## Methods Used

### Data Preprocessing
- The dataset was loaded and cleaned.
- Normalization was applied to ensure each feature contributed equally to the PCA.

### PCA (ACP)
- PCA was performed to reduce dimensionality and analyze the variance explained by the components.
- The cumulative variance helped determine how many components to retain for visualization and further analysis.

### Visualizations
- Scree plot (explained variance by component).
- Circle of correlations to interpret feature relationships.
- Projection of individuals (leaves) on the first two principal components, with class color-coding for intuitive grouping.

### Classification Insight
- Although the primary focus was on unsupervised analysis via PCA, visual clusters gave insights into potential class separability.
- Logistic regression was discussed but not applied, as the multiclass structure was better visualized than modeled in this context.

## Results & Insights

- PCA provided meaningful visual separations between certain leaf types based on just 2–3 components.
- The most influential descriptors in the principal components were **Solidity**, **Roundness**, and **Aspect Ratio**.
- Some classes clustered tightly, indicating the potential for successful supervised classification in a future extension of this work.

## Conclusion

This study showed the power of PCA in exploring complex image descriptor data and provided a solid foundation for further classification tasks. The analysis was kept aligned with the course content and demonstrated a thoughtful application of core data science principles in a visually interpretable way.

---

**Author:** Youssef Hamdani et Hamza Badreddine 
**Course:** Analyse de Donnee  
