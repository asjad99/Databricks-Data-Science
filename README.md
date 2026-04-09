### Data Science with Databricks 

This repository contains structured notes, guides, and references for developing expertise in the **Databricks platform** and implementing **end-to-end Machine Learning production systems**.

It focuses on practical aspects of **Machine Learning Operations (MLOps)** including governance, experimentation, deployment, monitoring, and automation within the Databricks ecosystem.

Databricks is essentially:

Spark + Delta Lake + MLflow + Cloud orchestration

Some notes can be found in Building Data Products with Databricks 

----

# 1. Dashboards 



----

# 2. Machine Learning

**A. Introduction, Big Picture and Fundamentals of ML In Databricks:**

This section focuses on the lifecycle of developing and deploying machine learning models: 

**Summary of Workflow**

- Book Appendix ML for developers [ML Process] 

**Further reading:**

- BLog post [Long intro to machine learning]()
- Paper [A Few Useful Things to Know About Machine Learning](https://homes.cs.washington.edu/~pedrod/papers/cacm12.pdf)
- Book Chapter [Chapter 5: Machine Learning Basics] 
- Book [Designing Machine Learning Systems]
- Paper [Machine Learning Operations (MLOps): Overview, Definition, and Architecture](https://epub.uni-bayreuth.de/id/eprint/7577/1/Machine_Learning_Operations_MLOps_Overview_Definition_and_Architecture.pdf)

TODO: add from .tex file 

Sections below describe more details around Core ML concepts and workflows:

### B. EDA and Data preprocessing
  
● Compute summary statistics on a Spark DataFrame using .summary() or dbutils data
summaries

● Remove outliers from a Spark DataFrame based on standard deviation or IQR

● Create visualizations for categorical or continuous features

● Compare two categorical or two continuous features using the appropriate method

● Compare and contrast imputing missing values with the mean or median or mode value

● Impute missing values with the mode, mean, or median value

● Use one-hot encoding for categorical features

● Identify and explain the model types or data sets for which one-hot encoding is or is not
appropriate.

● Identify scenarios where log scale transformation is appropriate


**Readings:**

- Book [Think Stats (For EDA)]
- CMU data visualization tips
  

### C. Model Development and Feature engineering

**Training a baseline model:**

● Identify how AutoML facilitates model/feature selection.

● Identify the advantages AutoML brings to the model development process

● Feature engineering Methods and workflows for extracting useful signals from raw data.


**Decision Trees and Ensemble Models:** 

● Use ML foundations to select the appropriate algorithm for a given model scenario

● Develop a training pipeline and  Training workflows

● Use common classification metrics: F1, Log Loss, ROC/AUC, etc

● Use common regression metrics: RMSE, MAE, R-squared, etc.

● Assess the impact of model complexity and the bias variance tradeoff on model
performance

● Perform cross-validation as a part of model fitting.


**Readings:** 

- Intro to statistical learning
- StatQuest: Decision Trees
- ML for developers chapter on decision trees 


### D. Model/Hyperparameter tuning  

● Compare estimators and transformers

● Use Hyperopt's fmin operation to tune a model's hyperparameters

● Perform random or grid search or Bayesian search as a method for tuning hyperparameters.

● Parallelize single node models for hyperparameter tuning

● Describe the benefits and downsides of using cross-validation over a train-validation split.

● Identify the number of models being trained in conjunction with a grid-search and
cross-validation process.

● Choose the most appropriate metric for a given scenario objective

● Identify the need to exponentiate log-transformed variables before calculating evaluation
metrics or interpreting predictions



####  E. Feature Store

● Identify the benefits of creating feature store tables at the account level in Unity Catalog in
Databricks vs at the workspace level

● Create a feature store table in Unity Catalog

● Write data to a feature store table

● Train a model with features from a feature store table.

● Score a model using features from a feature store table.

● Describe the differences between online and offline feature tables


- Evaluation strategies


### D. Real-World Machine Learning Challenges

Common issues encountered in production ML systems:
● Identify methods to mitigate data imbalance in training data

- Explainibility 
- Data drift
- Concept drift
- Training–serving skew
- Data quality issues
- Scalability challenges
- Monitoring and retraining strategies

![Real World ML](real-world-ml.png)

### F. MLflow, Model Registry & Reproducibility

Tools and practices for managing models in production.

● Identify the best practices of an MLOps strategy

● Identify the advantages of using ML runtimes

● Identify benefits of registering models in the Unity Catalog registry over the workspace
registry

● Identify scenarios where promoting code is preferred over promoting models and vice
versa

● Set or remove a tag for a model

● Promote a challenger model to a champion model using aliases

● Identify the best run using the MLflow Client API.

● Manually log metrics, artifacts, and models in an MLflow Run.

● Identify information available in the MLFlow UI

● Register a model using the MLflow Client API in the Unity Catalog registry

- Experiment tracking
- Reproducibility
- Model versioning
- Model registry
- ML lifecycle management
- Reproducible training pipelines
- Model promotion workflows (Dev → Staging → Production)

- Paper [MLflow: A Platform for Managing the Machine Learning Lifecycle]()
- Paper [KeystoneML: Optimizing Pipelines for Large-Scale Advanced Analytics]()

----

# 3. Handling Big Training datasets:

Spark for data preparation, model training, and deployment, while also gaining hands-on experience with Spark ML and pandas APIs on Spark. This course will introduce you to advanced concepts like hyperparameter tuning and scaling Optuna with Spark.

**Machine Learning Development with Spark**

- A Brief Overview of Spark Architecture for Machine Learning
- Introduction to Spark ML for Model Development
- Model Tracking and Packaging with MLflow and Unity Catalog on Databricks
- Model Development with Spark
- Model Tuning with Optuna on Spark
- Overview of Hyperparameter Tuning
- Introduction to Optuna on Spark
- Model Tuning with Optuna

**Advanced Machine Learning Operations**

- Overview of Machine Learning Operations on Databricks
- Review of MLOps
- Streamlining Development to Deployment
- Continuous Workflows for Machine Learning Operations
- Streamlining MLOps
- Streamlining MLOps with Databricks
- Testing Strategies with Databricks
- Automate Comprehensive Testing
- Model Rollout Strategies with Databricks
- Model Quality and Lakehouse Monitoring
- Introduction to Monitoring
- Lakehouse Monitoring
- Streamlining Multiple Environment Deployments - DABsBuild ML assets as CodeCourse Summary and Next Steps

---

# 4. MLOps in Databricks 

 CI/CD, pipeline management, and environment separation, while showcasing Databricks’ tools for automation and infrastructure management, such as Databricks Asset Bundles (DABs), Workflows, and Mosaic AI Model Serving. You will learn about monitoring, custom metrics, drift detection, model rollout strategies, A/B testing, and the principles of reliable MLOps systems, providing a holistic view of implementing and managing ML projects in Databricks.
 

### Model Monitoring & Observability

Building dashboards and monitoring systems for ML production environments.

Topics include:

- Model performance monitoring
- Data drift detection
- Feature distribution monitoring
- Data quality validation
- Observability dashboards
- Alerting systems

### Alerts & Automation 

Operational tooling for reliable ML systems.

Topics include:

- Automated testing pipelines
- Deployment automation
- System health monitoring
- Alerting mechanisms
- Migration and system upgrade support


----

# 5. Large Language Models (LLMs)

Notes and experiments related to:

- Prompt engineering
- LLM evaluation
- RAG pipelines
- LLM deployment patterns on Databricks

  

### Appendix A: Databricks

- [The Big Book of MLOps](https://blog.infocruncher.com/resources/ml-productionisation/The%20Big%20Book%20of%20MLOps%20(Databricks,%20v6,%202022).pdf)
- [MLOps workflows on Databricks](https://docs.databricks.com/aws/en/machine-learning/mlops/mlops-workflow)
- [Model deployment patterns](https://docs.databricks.com/aws/en/machine-learning/mlops/deployment-patterns)
- [Databricks Asset Bundles resources](https://docs.databricks.com/aws/en/dev-tools/bundles/resources)
- [GenAI](GenAI-Databricks.md)


### Appendix B: Resources

- [Designing machine learning systems](https://github.com/chiphuyen/dmls-book/blob/main/resources.md)
- [MLOps-Tools]()
- [IEEE MLOPS](https://ieeexplore.ieee.org/document/10081336)
- [CMU Machine Learning in Production](https://ckaestne.github.io/seai/)


# Appendix C: Platform Architecture

![](big_picture.png)

