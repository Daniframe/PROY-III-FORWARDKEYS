# Models for ForwadKeys
### Exploratory models / Association Rules
* Study of conditions on the cancellations .ipynb: Exploratory notebook where the idea for the relative frequency of cancellations from the deployment was developed. It also shows the conditions that lead to the most and least cancellations. It's deprecated and the import information is in the Deployment.
* Association_rules.Rmd: Study of rules to find which ones lead to the most and least cancellations. Similar to the python notebook but with association rules, it also derived in the creation of the deployment and basically is an outdated version of the deployment 

### Understading paxprofile models
* LDAPaxprofile.Rmd: Linear Discriminant Analysis model to understand via a surrogate interpretable model the variable "paxprofile", whcich is a defined as the ouput of an unkwown (and hence, considered a black box) model. Different approaches are tried: using only numerical variables, a mixture of numerical and categorical (one-hot encoded) variables, balancing the data, etc...
* DecisionTreePaxprofile.Rmd: Recursive partitioning decision trees using the rpart library to create an easy-to-interpret model that, as LDA, tries to understand the variable "paxprofile". Two models are built, one with the original data and the other with undersampling. There are some toy models playing with the error cost matrices, but they lose some of the main focus of the file.
* ROCCurves.Rmd: Comparison of the two previously mentioned models: LDA and RPT. They are compared via one-v-one ROC Curves. 
