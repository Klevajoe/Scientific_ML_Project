# Scientific_ML_Project

Multidimensional Outlier Detection 

Project Description: 

Detecting outliers in multivariate datasets can be challenging.  This is because in multiple dimensions there are several directions in which a point can be an outlier. When we think of outlier identification, it is easy to detect in 1-D (univariate), 2-D (bivariate), and more manageable in 3-D datasets. This is because of the visualization ease and available multivariate and/or statistical methods cater to the identification and possible removal of outliers in 1-D, 2-D spaces. However, 
outliers in oil and gas are both informative and important as it may be indicative of zones of high productivity i.e., sweet-spots, or regions of high petrophysical properties, which may inform drilling decisions. Additionally, most petroleum datasets are multidimensional making it susceptible to the curse of dimensionality, which makes outlier identification a non-trivial task since highly dimensional spaces cannot be visualized without appropriate dimensionality reduction methods. The coupling effect of the curse and outliers in multidimensional datasets makes outlier identification crucial given it may lead to erroneous inferences and decision-making if machine learning models are built on such data without appropriate preprocessing or lead to identifying sweet-spots areas.

To this end, we propose to use an autoencoder architecture to identify and detect multivariate outlier samples in a space of low dimensionality i.e., the latent space with an appropriate cost function. Afterwards, we will then compare our methods with existing methodologies for multivariate outlier detection such as isolation forest, DBSCAN on high-dimensional data, and local outlier factor methods  with PCA visualizations on a toy dataset as ground truth, then apply it to actual petroleum datasets. We hypothesisze that our proposed method will be more robust and generalizable across multiple dimensions. 


Goals:

1. Generate a toy dataset with multivariate outliers across different dimensions as ground truth to test the methodology
2. Train an Autoencoder neural network and characterize the latent space per distributions.
3. Propose a metric that serves as a threshold to identify outliers in multidimensional spaces.
4. Compare to other detection methods mentioned in the project’s description.
5. Perform workflow on real-world dataset with direct application in the production of oil and gas using sucker rod pumps posed as a classification problem.

Link to data:

Github data repository:  https://github.com/JoseLuisHerme/Scientific_ML_Project/blob/main/rodpump_failure%202.csv

About the data:

This is a petroleum dataset obtained from a variety of rod pump production equipment at an oil field located in North Dakota. The multidimensional dataset consists of 25 features and 2597 samples. There are 24 predictor features (both categorical and numerical) and a response feature, failure type, which correspond to failure types that can occur when producing oil and gas wells.

References

1. Shevlyakov, G., Andrea, K., Choudur, L., Smirnov, P., Ulanov, A., & Vassilieva, N. (2013, May). Robust versions of the Tukey boxplot with their application to detection of outliers. In 2013 IEEE International Conference on Acoustics, Speech and Signal Processing (pp. 6506-6510). IEEE.
Chen, Z., Yeo, C. K., Lee, B. S., & Lau, C. T. (2018, April). Autoencoder-based network anomaly detection. In 2018 Wireless telecommunications symposium (WTS) (pp. 1-5). IEEE.
2. Tukey, J. W. (1977). Exploratory data analysis (Vol. 2, pp. 131-160).
3. Mahalanobis, P. C. (1936). On the generalised distance in statistics. In Proceedings of the national Institute of Science of India (Vol. 12, pp. 49-55).
4. van Beekveld, M., Caron, S., Hendriks, L., Jackson, P., Leinweber, A., Otten, S., ... & White, M. (2021). Combining outlier analysis algorithms to identify new physics at the LHC. Journal of High Energy Physics, 2021(9), 1-33.
5. Liu, F. T., Ting, K. M., & Zhou, Z. H. (2008, December). Isolation forest. In 2008 eighth ieee international conference on data mining (pp. 413-422). IEEE
6. Breunig, M. M., Kriegel, H. P., Ng, R. T., & Sander, J. (2000, May). LOF: identifying density-based local outliers. In Proceedings of the 2000 ACM SIGMOD international conference on Management of data (pp. 93-104).
