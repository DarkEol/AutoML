# AutoML-Ontology

The process of creation and use of the ontology is made in three steps that are the same for all AutoML libraries being used:

1. XXX_Meta - preparation of the training meta-data. At this step, the extraction of meta-features from training datasets is made along with the search for the best model suggested for a given task by the considered AutoML library. The results are saved as CSV and XLSX (Excel) files.

2. XXX_DecisionTree - preparation of the ontology. The meta-data that was obtained in the previous step is used for creation of the ontology. The ontology is created by traversing a decision tree that is built from meta-features with the suggested algorithm as a target.

3. XXX_MetaOnto - the use of the ontology. In this final step, the created ontology is used. The search for the best model for a given dataset by the considered AutoML library is made in three different modes: 1)only time constrain, 2)time constrain and early stopping, 3)time constrain, early stopping and use of a subset of algorithms suggested by the ontology.
