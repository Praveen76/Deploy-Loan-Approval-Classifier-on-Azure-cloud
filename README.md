# Deploy-Loan-Approval-Classifier-on-Azure-cloud

In this project, I'll walk you through deploying any Machine Learning project, Loan Approval Classifier model in our case, on Azure Cloud.

Deploy Loan Approval Classifier on Azure cloud.

# **Directory Structure**
 * Data: Data used for this project. However Train/DataPrep.py will be used to import real time data from Database for our this project.
 * configs:
	    * configs/config.yaml: Stores DB server's credentials.
	    * configs/env.yml : Dependencies that need to be installed for this project.
 * Train: It contains python scripts that will be utilized for Model training.
	    * Train/DataPrep.py : Import Data from DB and preprocess it.
	    * Train/model.py :  Python script for model training and export pickle file to outputs directory.

* outputs : Stores various output and pickle files such as Encode,pre-processor used in training step, Trained Model,etc.

* Prediction: It contains python scripts that will be utilized to predit test, or actual data.
      * prepare.py: Preprocess and predict response variable for test data
      * score.py: Azure script file.
* Performance: It contains python scripts that will be utilized to assess model performance on actual data and performance across different run_Ids over the time.
      * FindActuals.py: Calculate model performance and store logs in Database.
      * Performance/modelPerformance.py: Calculate model performance over the time across different run_Ids to check model or data drift.

* utils.py: It contains different utility functions.
* main.py: Python script to define order to follow to execute different relavant Azure experiment scripts.
* requirements.txt: Python dependencies that will be required to be installed to run this project.

# **Instructions for Installation:**
**Dependencies:**
* joblib>= 0.16
* scikit-learn>=0.23
* pandas>= 1.0
* numpy>=1.1
* pyodbc==4.0.30
* urllib3==1.25.9
* sqlalchemy==1.3.18
* pyyaml>=5.3
* azureml-sdk>=1.18.0

The code has been tested on Windows system. It should work well on other distributions but has not yet been tested.

In case of any issue with installation or otherwise, please contact me on [Linkedin](https://www.linkedin.com/in/praveen-kumar-anwla-49169266/)


# **About Me:**
I’ve been working as a Data Scientist for a very long time now. I've worked on various NLP, Machine learning & cutting edge deep learning frameworks to solve business problems. Please feel free to check out my personal wesbsite [TowardsMachineLearning.Org](https://towardsmachinelearning.org/) , where I cover an array of topics from Machine learning, NLP, Deep Learning, etc.




