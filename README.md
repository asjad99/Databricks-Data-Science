### Data Science in Cloud 

This repository contains structured notes, guides, and references for developing expertise in the **Databricks platform** and implementing **end-to-end Machine Learning production systems**.

It focuses on practical aspects of **Machine Learning Operations (MLOps)** including governance, experimentation, deployment, monitoring, and automation within the Databricks ecosystem.

Databricks is essentially:

Spark + Delta Lake + MLflow + Cloud orchestration

Some notes can be found in Building Data Products with Databricks 

# 1. Dashboards 



----

# 2. Machine Learning


**Introduction and Fundamentals:**

This section focuses on the lifecycle of developing and deploying machine learning models.


- BLog post [Long intro to machine learning]()
- Paper [A Few Useful Things to Know About Machine Learning](https://homes.cs.washington.edu/~pedrod/papers/cacm12.pdf)
- Book Chapter [Chapter 5: Machine Learning Basics] 
- Book [Think Stats (For EDA)]
- Book Appendix [ML Process] 
- Book [Designing Machine Learning Systems]
- Paper [Machine Learning Operations (MLOps): Overview, Definition, and Architecture](https://epub.uni-bayreuth.de/id/eprint/7577/1/Machine_Learning_Operations_MLOps_Overview_Definition_and_Architecture.pdf)

TODO: add from .tex file 



### Data preprocessing


###  Feature engineering


### Modeling and Hyperparameter tuning 

Core ML concepts and workflows including:

- Feature engineering Methods and workflows for extracting useful signals from raw data.

Topics include:
        - Feature engineering pipelines
        - Feature stores

- Training workflows
- Evaluation strategies




## Real-World Machine Learning Challenges

Common issues encountered in production ML systems:

- Data drift
- Concept drift
- Training–serving skew
- Data quality issues
- Scalability challenges
- Monitoring and retraining strategies

![Real World ML](real-world-ml.png)

## MLflow, Model Registry & Reproducibility

Tools and practices for managing models in production.

- Experiment tracking
- Reproducibility

  - Model versioning
  - Model registry
- ML lifecycle management
- Reproducible training pipelines
- Model promotion workflows (Dev → Staging → Production)


- Paper [MLflow: A Platform for Managing the Machine Learning Lifecycle]()
- Paper [KeystoneML: Optimizing Pipelines for Large-Scale Advanced Analytics]()


## Handling Big Training datasets:

Spark for data preparation, model training, and deployment, while also gaining hands-on experience with Spark ML and pandas APIs on Spark. This course will introduce you to advanced concepts like hyperparameter tuning and scaling Optuna with Spark.

---

# 3. MLOps in Databrikcs 

 CI/CD, pipeline management, and environment separation, while showcasing Databricks’ tools for automation and infrastructure management, such as Databricks Asset Bundles (DABs), Workflows, and Mosaic AI Model Serving. You will learn about monitoring, custom metrics, drift detection, model rollout strategies, A/B testing, and the principles of reliable MLOps systems, providing a holistic view of implementing and managing ML projects in Databricks.

 

# Model Monitoring & Observability

Building dashboards and monitoring systems for ML production environments.

Topics include:

- Model performance monitoring
- Data drift detection
- Feature distribution monitoring
- Data quality validation
- Observability dashboards
- Alerting systems

**Alerts & Automation**

Operational tooling for reliable ML systems.

Topics include:

- Automated testing pipelines
- Deployment automation
- System health monitoring
- Alerting mechanisms
- Migration and system upgrade support


----

# 4. Large Language Models (LLMs)

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

