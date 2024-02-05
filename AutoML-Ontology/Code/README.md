# AutoML-Ontology

The process of creation and use of the ontology is made in three steps same for all AutoML libraries being used:

1. XXX_Meta.ipynb - preparation of the training meta-data. At this step extraction of meta-features from training datasets is made along with search for a best model suggested for a given task by the considered AutoML library.

2. XXX_DecisionTree - preparation of the ontology. The meta-data that was obtained at the previous step is used for creation of the ontology. The ontology is created by traversing a decision tree that is built from meta-features with suggested algorithm as a target.

3. XXX_MetaOnto - the use of the ontology. At this final step the created ontology is used. The search for the best model for a given dataset by the considered AutoML library is made in three different modes: 1)only time constrain, 2)time constrain and early stopping, 3)time constrain, early stopping and subset of algorithms suggested by ontology.
