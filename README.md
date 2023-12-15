# DuplicateDetection
This code performs a scalable duplicate detection method for Web Shop products. 
It uses title-modelwords based representations of the products and performs LSH in combination with a multi-component similarity method.

# Load the data
replace the path with your own path

# descriptions
descriptions creates a dictionary of separate product descriptions

# preprocess
in the preprocessing step, the representations of inch, hertz and pound are changed to the same string. Furthermore everything is converted to lower case and the brackets are removed.


# modelwords
the modelwords are extracted from the titles to create a set of modelwords

# binarymatrix
The modelwords are used to create binary representations of the products

# Minhash
Turns binary matrix into signature matrix,, with unique signatures for each product

# LSh
creates candidate pairs using the signatures, to decrease the number of pairs to be evaluated.

# qgrams and jaccard
Similarity measures that are later used for classification

# brands
The brands are extracted from the data

# finalcandidates
Here an extra cleaning step is performed to remove irrelevant alternatives and classification is performed t obtain final pairs

# All duplicates and True positives 
are later needed and hence defined here

# Getmetrics
the evaluation metrics are computed with this function

# splitdata
used to split the data in test and train set

# Bootstrap
Here a bootstrap of 5 bootstraps is ran. Hyperparameters can be manually specified and the set over which rows and bands are searched as well. The evaluation measures are computed and averaged over bootstraps.The results are printed and in the next block there are plots generated.
