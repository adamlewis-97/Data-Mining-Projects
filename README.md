This repo contains two self-contained data-mining projects:

Basel Climate Clustering - a tabular workflow that utilises 10 years of daily weather observations, performs correlation-based feature selection, outlier filtering, PCA for dimensionality reduction, and compares k-means vs. DBSCAN to uncover seasonal weather regimes.

Image Embedding & Classification - a deep-learning-powered pipeline that extracts 512-D ResNet-18 embeddings for the Oxford-IIIT Pets and Food-101 datasets, visualises latent spaces via PCA + t-SNE, applies unsupervised clustering (k-means, hierarchical, DBSCAN), and evaluates supervised classifiers (logistic regression, k-NN, linear/RBF SVM with GridSearchCV).

Each task includes commented Jupyter notebooks, evaluation metrics (silhouette scores, Davies–Bouldin index, confusion matrices), and a pickled SVM model for Food-101. Follow the setup instructions below to reproduce results or adapt the pipelines to your own datasets.

