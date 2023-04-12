# Machine Learning Based Prediction For Hierarchical Disease Classification
Using ML to predict diseases from symptoms, with the hierarchy of diseases.
The methodology in the project consists of Dataset selection, proper data preprocessing, and then using the required classifiers and predictors to get the desired outcome. The training Dataset is selected from Kaggle, where the columns were having symptoms and the rows were having the diseases, with cells having binary
values. We also dropped some rows and columns which were irrelevant to model. In data pre-processing, we tried searching the available disease and their known
hierarchy from the Disease Ontology website. We manually tried finding the hierarchy
of diseases of the test dataset. We created the Hierarchy at two levels. In level 1, we
got three classes, immunological, degenerate, and genetic. In level 2, we further divided
the immunological, degenerate, and genetic diseases into 4, 8 and 1
sub class respectively. The methodology in the project consists of Dataset selection, proper data
preprocessing, and then using the required classifiers and predictors to get the desired
outcome. The training Dataset is selected from Kaggle, where the columns were having
symptoms and the rows were having the diseases, with cells having binary
values. We also dropped some rows and columns which were irrelevant to model.
In data pre-processing, we tried searching the available disease and their known
hierarchy from the Disease Ontology website. We manually tried finding the hierarchy
of diseases of the test dataset. We created the Hierarchy at two levels. In level 1, we
got three classes, immunological, degenerate, and genetic. In level 2, we further divided
the immunological, degenerate, and genetic diseases into 4, 8 and 1
sub class respectively. Also like for degenerate subclasses, we created a new dataset with rows relating only
to that class, removing rows from degenerate and genetic class, hence increasing
efficiency and saving resources. Creating a dataset at each level will remove the
problem of information loss.
We used 17 classifiers in total at different levels to traverse through the hierarchy to
reach the target disease to predict. And at the nodes we used predictors to predict the
Disease and its hierarchy.
The last column of the dataset was in string format, so we used a label encoder to
convert the values from categorical values into numerical values.
