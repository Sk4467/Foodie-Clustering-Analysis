# Foodie-Clustering-Analysis
Utilize NLP to uncover restaurant patterns and cuisines through advanced clustering analysis.

## Dataset:
https://drive.google.com/file/d/1cePdYOEIFQv0gFcH4UV2-DcbXVX-kE7a/view?usp=drive_link

## Problem Statement

The goal of the NLPFoodieClustering project is to find competitive stores or restaurants that offer similar food items at comparable prices. Additionally, we aim to identify food items or restaurants with prices significantly higher or lower compared to other menu items or competitors.

## Approach

1. **Data Preprocessing**: The dataset contains columns for food items, descriptions, restaurants, and prices. We merge the item and description columns to create a single item representation. This step ensures a comprehensive view of the food items for further analysis.

2. **Word Embeddings**: Utilizing Natural Language Processing (NLP) techniques, we convert the food items' textual data into word embeddings. Specifically, we employ word embedding models like Word2Vec or FastText to capture semantic meanings and relationships between food items.

3. **Dimensionality Reduction**: To visualize and cluster the food items effectively, we apply dimensionality reduction techniques like t-SNE, SVD, or PCA to reduce the high-dimensional word embeddings into a lower-dimensional space while preserving essential patterns.

4. **Visualization**: We create visualizations of the embeddings to gain insights into the distribution and relationships of food items in the reduced dimensional space. This visualization provides a better understanding of the data and potential clustering patterns.

5. **Clustering**: Next, we use K-means clustering or other suitable algorithms to group similar food items together based on their embeddings. This step helps us identify competitive stores offering similar items at similar prices.

6. **Price Categorization**: Within each cluster, we categorize the food items' prices into "high," "medium," and "low" ranges. This allows us to compare the pricing of different menu items within the same cluster.

7. **Outlier Identification**: Based on the price categorization, we detect food items or restaurants with prices significantly higher or lower than their cluster's average. These outliers may indicate potential areas for price adjustment or investigation of competitive pricing strategies.

## Requirements

Before running the project, ensure you have the following dependencies installed:

- Python (>= 3.6)
- NumPy
- Pandas
- NLTK
- Gensim
- scikit-learn
- Matplotlib (for visualizations)

## Usage

1. Ensure that the raw data is placed in the `data` folder, following the format specified in `raw_data.csv`.

2. Run the notebooks in the `notebooks` folder sequentially. These notebooks will guide you through data preprocessing, word embeddings, dimensionality reduction, visualization, clustering, and outlier identification.

3. Analyze the results obtained from clustering and outlier detection to identify competitive stores and items with pricing opportunities.

## Conclusion

The NLPFoodieClustering project demonstrates how NLP techniques, dimensionality reduction, and clustering can be used to identify competitive stores offering similar food items at similar prices. The visualization and outlier detection provide valuable insights into potential areas for price adjustments and competitive pricing strategies.

For any questions or feedback, feel free to reach out to the project maintainers.

Happy clustering and exploring the world of competitive food businesses!
