# AutoML-Framework 

AutoML-Framework that unites several popular AutoML tools. Different AutoML libraries that use Scikit-Learn as a source of algorithms cannot run together because of their dependency on different versions of libraries; in particular, Auto-Sklearn can run together, neither with TPOT nor with Hyperopt-Sklearn. Therefore, two separate components were developed within the Framework: one unites Auto-Sklearn and H2O, and the other works with TPOT, Hyperopt-Sklearn, and H2O.

The Framework takes as input the dataset, the ratio in which the data has to be split into train and test sets and the time limit that each used AutoML library is allocated to perform the search. Then, each AutoML library runs in a separate thread with given data and limits. After the search is done, the results are summed up in a common table. The general architecture of the Framework is shown in Fig. 1.

![AutoML Framework architecture!](framework.png "AutoML Framework architecture")

The Framework contains the following modules:

**Data extraction module.** The data extraction module extracts the data to be processed. Users can load the data either from the open repository OpenML.org by dataset ID or from a local CSV file provided as input. The data is stored as a DataFrame in the Pandas library, and all preprocessing modules receive the same data.

**Data preprocessing module.** Each AutoML library requires attributes and targets to be presented in a specific form in order to perform a search, e.g. the target for the classification task should be categorical. This module checks input data and performs transformation should the need arise. At this step, the data is also split into training and test sets with the same ratio for all used libraries.

**Search module.** After the data is prepared and split, the training set and the information about the target are forwarded to the search module. The search module performs a parallel search for a machine learning model in all used AutoML libraries while taking into account the same limits, e.g., running time.

**Result interpretation module.** Once the models are found, the test set is used to calculate the common performance metrics of the models. 

**Uniting module.** After the metrics of models found by all AutoML libraries are calculated, they and information about the models are stored in a common results table, which can then be saved as .xlsx (Excel) file.

The work of the Framework can be started by calling the function "runAutoML". This function has three parameters:
1. Dataset – if the parameter is numeric, then it means ID in the OpenML repository; if it is a string, then the name of CSV file;
2. Time – maximum running time allocated for a search (integer, number of seconds);
3. Ratio – split ratio for division data into train and test sets (real number between 0 and 1, the ratio of the training set).

Examples of Framework launch:
- runAutoML("IBM-Employee.csv", 300, 0.75) – load data from file "IBM-Employee.csv”, divide into 3/4 training and 1/4 test sets and perform search for 5 minutes.
- runAutoML(4153, 900, 0.80) - load the dataset with the ID 4153 from OpenML, split into 4/5 training and 1/5 test sets and perform search for 15 minutes.
