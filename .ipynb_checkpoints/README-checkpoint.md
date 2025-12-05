# Iris-Classification

## Problem Statement
- This is a dataset that contains 150 rows of data about different species of Iris flowers. There is an equal number of rows for each species. 

- The purpose of this analysis is to create a model to accurately predict the species based on the petals and sepals. 

## Data Dictionary

| Column Name | Description |
|-------------|-------------|
| **sepal_length** | Length of the sepal of the flower (cm).                          |
| **sepal_width**  | Width of the sepal of the flower (cm).                           |
| **petal_length** | Length of the petal of the flower (cm).                          |
| **petal_width**  | Width of the petal of the flower (cm).                           |
| **species**      | Species of the iris flower (setosa, versicolor, virginica). |

## Executive Summary

### Data Cleaning Steps
No data cleaning had to be performed on this dataset. 

### Key Visualizations
Include key visualizations that highlight important aspects of the data. Use graphs, charts, or any other visual representation to make your points.

#### Visualization 1: [Pairplot of the Columns]
This shows all the scatterplots of the different features for the petals and sepals. It also shows histograms of each feature. 

![pairplot](./images/pairplot.png)

#### Visualization 2: [Petal Length]
In this histogram, we can clearly see that Setosas' petal length only ranges from 1-2 cm, and there is a considerable gap between Setosas and the other 2 species, Versicolor, which ranges from 3-5.5 cm, and Virginica, which ranges from 4-7 cm.

Versicolor and Virginica have some overlap, but Setosa is in its own area.

![petal length](./images/petal_length_hist.png)

#### Visualization 3: [Petal Width]
Similar to Petal Length, there are more obvious separations between the different species. The Septosa range goes from 0-0.5 approximately. There is a decent gap between Setosa and the other 2 speciers. Versicolor have a range from around 0.75-2, and Virginica goes from 1-2.5, causing an overlap.

![petal width](./images/petal_width_hist.png)

#### Visualization 4: [Sepal Width]
The Sepal Width seems to have the most overlap between the 3 species. Setosa has a range from 2-4.5 cm (highest of the 3 species), Versicolor with a range from 2-3.5 cm, and Virginica's range is 2-4 cm.

![sepal width](./images/sepal_width_hist.png)

#### Visualization 5: [Sepal Length]
Unlike with Petal Length, all 3 species overlap in this histogram. The Setosa range for sepal length is from ~4.5-6 cm, Versicolor from ~4.5-7.5 cm, and Virginica ~4.5-8 cm. While they all have the same length on the low side, their higher ranges are different, so the distribution for each overlap, but they all have different peaks and different widths, means they have different means and standard deviations.

![sepal length](./images/sepal_length_hist.png)

## Conclusions/Recommendations

I trained Logisitic Regression, Random Forest, and K Nearest Neighbors (KNN) models with the data. The results are below.

| Model | Accuracy | 
| ----- | ----- |
| Logistic Regression | 0.97 | 
| Random Forest | 0.95 |
| KNN | 1 |

KNN had the best score, accurately predicting the species of iris flower 100% of the time. Normally, this would be a concern of overfitting, however, since the dataset is so small, a score that high shouldn't be any cause for concern. 

Confusion Matrix of Test Set for KNN

![confusion matrix](./images/knn_conf.png)

## Additional Information
Include any additional information, references, or resources that might be relevant for understanding the analysis.

---

Feel free to replace the placeholders with your actual content. Additionally, if you have images for your visualizations, make sure to replace the placeholder paths with the correct file paths or URLs.

Once you've filled in the content, save the file with a `.md` extension (e.g., `README.md`). You can use this Markdown file on platforms like GitHub to provide a well-structured README for your analysis.
