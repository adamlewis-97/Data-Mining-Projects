This repo contains two self-contained data-mining projects:

Basel Climate Clustering - a tabular workflow that utilises 10 years of daily weather observations, performs correlation-based feature selection, outlier filtering, PCA for dimensionality reduction, and compares k-means vs. DBSCAN to uncover seasonal weather regimes.

Image Embedding & Classification - a deep-learning-powered pipeline that extracts 512-D ResNet-18 embeddings for the Oxford-IIIT Pets and Food-101 datasets, visualises latent spaces via PCA + t-SNE, applies unsupervised clustering (k-means, hierarchical, DBSCAN), and evaluates supervised classifiers (logistic regression, k-NN, linear/RBF SVM with GridSearchCV).

Each task includes commented Jupyter notebooks, evaluation metrics (silhouette scores, Davies–Bouldin index, confusion matrices), and a pickled SVM model for Food-101. Follow the setup instructions below to reproduce results or adapt the pipelines to your own datasets.

## Datasets

The notebooks expect three data sources, each in its own subfolder under `data/`:

### Basel Climate Data 

1. Go to <https://www.meteoblue.com/en/weather/archive/export>.
2. Select **Basel, Switzerland** as the location.
3. Set the date range to 2010-01-01 … 2019-12-31.
4. Choose **Daily** resolution.
5. Click **Download CSV**.
6. Rename the file to `basel_weather_2010_2019.csv` and place it in `data/climate/`.

### Food-101 
   - **Source**: Kaggle “Food-101” dataset  
   - **Download link**: https://www.kaggle.com/datasets/dansbecker/food-101  
   - **Place unzipped files** under:
     ```
     data/food101/images/
     data/food101/meta/
     ```

### Oxford-IIIT Pets  
   - **Source**: University of Oxford “IIIT Pets”  
   - **Download link**: https://www.robots.ox.ac.uk/~vgg/data/pets/  
   - **Place unzipped files** under:
     ```
     data/pets/images/
     data/pets/annotations/
     ```


