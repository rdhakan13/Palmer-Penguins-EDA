# Palmer Penguins ML Classification

## About the data
Data were collected by Dr. Kristen Gorman and the Palmer Station, Antarctica LTER, a member of the Long Term Ecological Research Network [^1].

The palmerpenguins package contains two datasets:
- penguins: Simplified version of the raw data.
- penguins_raw: Contains all original variables and names.

Both datasets contain data for 344 penguins, across 3 species from 3 islands in the Palmer Archipelago, Antarctica. A subset of this data, containing 6 of 8 attributes (as shown in the below table), and 333 of 344 items (excluding items with 1 or more null attributes) was used for machine learning classification of the penguin species. 

| Attributes               | Values                    |
|--------------------------|---------------------------|
| Species                  | Adelie, Chinstrap, Gentoo |
| Bill Length (BL) / mm    | 32.1 - 59.6               |
| Bill Depth (BD) / mm     | 13.1 - 21.5               |
| Flipper Length (FL) / mm | 172 - 231                 |
| Body Mass (BM) / g       | 2700 - 6300               |
| Sex                      | Male, Female              |

The methodology of this project involved the below, which is summarised in a greater depth in `Penguins Report.pdf` file:
1. Exploratory Data Analysis (EDA) - to understand the distribution of the species in the sample data and understand the distribution of the four continuous attributes.
2. Unsupervised Learning - Using UMAP data projection with K-Means to classify penguins with unlabelled data
3. Supervised Learning - A comparative study between the baseline (uniform), KNN and Random Forest models using cross-validation macro-averaged F1 score. 

[^1]: Horst AM, Hill AP, Gorman KB (2020). palmerpenguins: Palmer Archipelago (Antarctica) penguin data. R package version 0.1.0. https://allisonhorst.github.io/palmerpenguins/. doi: 10.5281/zenodo.3960218.
