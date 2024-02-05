# AutoML
This repositiry is devoted to AutoML related projects:

**AutoML-Framework** contains project of uniting several common used AutoML libraries under umbrella of a common framework that enables the use of common constraints and metrics. This enables to compare models created in same constraints by different AutoML tools.
Currently the Framework makes use of the following AutoML libraries: Auto-sklearn, H2O, TPOT, Hyperopt-sklearn. 

**AutoML-Ontology** containts project aimed to speed up the search in the hyperparametes space by limiting the search space by the most promising algorithms for a given task. The suggestions of algorithms is made based on meta-features of previously proccesed datasets. The connection between meta-features and best algorithms are captured and stored in ontology for a later retrivial. 
