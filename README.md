# 8 Feature Engineering Techniques:

Feature Engineering is really important for improving the performance of your machine-learning models. It is necessary to decrypt how humans understand the data. Humans tend to find complex patterns or relations and recognize them, even when they don't exist.

Deconstructing is an "ART"

1. Imputation:

It deals with handling missing values in data. While deleting records that are missing certain values is one way of dealing with this issue, it could also mean losing out on a chunk of valuable data. This is where imputation can help. It can be broadly classified into two types. Such as:

Categorical Imputation: Missing categorical values are generally replaced by the most commonly occurring value in other records.
Numerical Imputation: Missing numerical values are generally replaced by the mean of the corresponding value in other records.

2. Discretization

It involves essentially taking a set of values of data and grouping sets of them together in some logical fashion into bins (or buckets). Binning can apply to numerical values as well as to categorical values. This could help prevent data from overfitting but comes at the cost of loss of granularity of data. The grouping of data can be done as follows:

a) Grouping of equal intervals
b) Grouping based on equal frequencies (of observations in the bin)
c) Grouping based on decision tree sorting (to establish a relationship with target)

3. Categorical Encoding

Categorical encoding is the technique used to encode categorical features into numerical values which are usually simpler for an algorithm to understand. One hot encoding(OHE)  is a popularly used technique of categorical encoding. Here, categorical values are converted into simple numerical 1’s and 0’s without the loss of information. As with other techniques, OHE has its disadvantages and has to be used sparingly. It could result in a dramatic increase in the number of features and result in the creation of highly correlated features. 

Besides OHE there are other methods of categorical encodings, such as 
1. Count and Frequency encoding- captures each label's representation,
2. Mean encoding -establishes the relationship with the target and
3. Ordinal encoding- the number assigned to each unique label.

4. Feature Splitting

Splitting features into parts can sometimes improve the value of the features toward the target to be learned. For instance, in this case, Date better contributes to the target function than Date and Time.

5. Outliers are unusually high or low values in the dataset which are unlikely to occur in normal scenarios. Since these outliers could adversely affect your prediction they must be handled appropriately. The various methods of handling outliers include:

a. Removal: The records containing outliers are removed from the distribution. However, the presence of outliers over multiple variables could result in losing out on a large portion of the datasheet with this method.
b. Replacing values: The outliers could alternatively be treated as missing values and replaced by using appropriate imputation.
c. Capping: Capping the maximum and minimum values and replacing them with an arbitrary value or a value from a variable distribution.
d. Discretization

6. Variable Transformations
Variable transformation techniques could help with normalizing skewed data. One such popularly used transformation is the logarithmic transformation. Logarithmic transformations operate to compress the larger numbers and relatively expand the smaller numbers. This in turn results in less skewed values especially in the case of heavy-tailed distributions. Other variable transformations used include Square root transformation and Box cox transformation which is a generalization of the former two.

7. Scaling 
Feature scaling is done owing to the sensitivity of some machine learning algorithms to the scale of the input values. This technique of feature scaling is sometimes referred to as feature normalization. The commonly used processes of scaling include:

Min-Max Scaling: This process involves the rescaling of all values in a feature in the range 0 to 1. In other words, the minimum value in the original range will take the value 0, the maximum value will take 1 and the rest of the values in between the two extremes will be appropriately scaled.
Standardization/Variance scaling: All the data points are subtracted by their mean and the result is divided by the distribution's variance to arrive at a distribution with a 0 mean and variance of 1.
It is necessary to be cautious when scaling sparse data using the above two techniques as it could result in additional computational load.

8. Creating Features
Feature creation involves deriving new features from existing ones. This can be done by simple mathematical operations such as aggregations to obtain the mean, median, mode, sum, or difference and even product of two values. These features, although derived directly from the given data, when carefully chosen to relate to the target can have an impact on the performance(as demonstrated later!)

While the techniques listed above are by no means a comprehensive list of techniques, they are popularly used and should help you get started with feature engineering in machine learning.




