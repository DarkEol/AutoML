# AutoML
This repository is devoted to AutoML-related projects:

**AutoML-Framework** is a project that unites several commonly used AutoML libraries under the umbrella of a common framework that enables the use of common constraints and metrics. This enables us to compare models created under the same constraints by different AutoML tools. Currently, the Framework makes use of the following AutoML libraries: Auto-sklearn, H2O, TPOT, and Hyperopt-sklearn.

**AutoML-Ontology** is a project aimed to speed up the search in the hyperparameters space by limiting the search space to the most promising algorithms for a given task. The algorithm suggestions are made based on meta-features of previously processed datasets. The connection between meta-features and best algorithms is captured and stored in ontology for later retrieval.
