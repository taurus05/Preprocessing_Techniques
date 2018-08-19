# Preprocessing_Techniques
Data Preprocessing is considered as one of the most challenging areas in the field of data science. There is very important reason behind doing this:
* It increases model effeciency.
* Helps in bringing the data values in a specific range, so that no feature value dominates the ML model.
* Getting insinghts into what kind of data is present, also helps in selection of appropriate ML model.
* If missing values are encountered, then they can be handeled accordingly.
* It becomes a lot easier to select the type of learning to be performed on that data set(Supervised if labels are present, else unsupervised).

All the above mentioned points are the outcomes of applying a good preprocessing technique. But in some cases, missing values might be present in the dataset, which can cause unexpected behaviour of ML model in both training and testing phases.
Hence, missing values should be handled very carefully. Missing values are handled in following way:
1. Statistical Approach
  * If the data values for a particular feature are continuous, then missing value can be substituted with the mean of the         values along that column
  * If the data values for a particular feature are discrete, i.e. it has value from a specific set of values, then using the       most frequently occouring value can be used to substitute the missing values.
  * If the data values obey gaussian distribution, then we can substitute it with the median of the values along that column.
2. Machine Learning model based missing value Imputation
    This is amongst the most emerging areas. The most important aspect of this approach is that, without even running a ML         model predictions for missing values can be made. It lies at the intersection of supervised and unsupervised Approach.
    Major steps involved in this approach are :
    1. Seperation of tuples (row) values in dataset, on the basis of complete or incomplete.
    1. Clustering of complete dataset, to determine standard deviation and cluster centroid for each class.
    1. Imputing missing values using these results.
 
There are several research papaers published showing how such problem can be solved. In this Jupyter Notebook, I have used results of a research paper to verify the results obtained using Imputation technique with that of the complete dataset.
