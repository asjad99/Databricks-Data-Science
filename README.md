### Data Science in Cloud 

This repository contains structured notes, guides, and references for developing expertise in the **Databricks platform** and implementing **end-to-end Machine Learning production systems**.

It focuses on practical aspects of **Machine Learning Operations (MLOps)** including governance, experimentation, deployment, monitoring, and automation within the Databricks ecosystem.


# Platform Architecture

![](big_picture.png)


## Unity Catalog & Data Governance

Key components for managing data and model assets within Databricks.

Topics include:

- **Kimball Data Modeling**
- **Medallion Architecture**
  - Bronze → Silver → Gold data layers
- **Unity Catalog**
  - Access control and permissions management
  - Data lineage tracking
  - Model lineage tracking
- **Data governance**
- **Model governance**

# Machine Learning

TODO: add from blog posts, .tex file 

This section focuses on the lifecycle of developing and deploying machine learning models.

## Fundamentals

Core ML concepts and workflows including:

- Feature engineering
- Training workflows
- Evaluation strategies
- Experiment tracking
- Reproducibility

## Large Language Models (LLMs)

Notes and experiments related to:

- Prompt engineering
- LLM evaluation
- RAG pipelines
- LLM deployment patterns on Databricks

## Real-World Machine Learning Challenges

Common issues encountered in production ML systems:

- Data drift
- Concept drift
- Training–serving skew
- Data quality issues
- Scalability challenges
- Monitoring and retraining strategies

![Real World ML](real-world-ml.png)

## Model Registry & Reproducibility

Tools and practices for managing models in production.

- **MLflow**
  - Experiment tracking
  - Model versioning
  - Model registry
- ML lifecycle management
- Reproducible training pipelines
- Model promotion workflows (Dev → Staging → Production)

# Jobs & Pipelines

Automation and orchestration of ML workflows in Databricks.

Topics include:

- Databricks Jobs
- Training pipelines
- Batch and real-time inference workflows
- Pipeline orchestration
- Feature pipelines
- Model serving in production environments
- Integration with external systems

# Model Monitoring & Observability

Building dashboards and monitoring systems for ML production environments.

Topics include:

- Model performance monitoring
- Data drift detection
- Feature distribution monitoring
- Data quality validation
- Observability dashboards
- Alerting systems

# Alerts & Automation

Operational tooling for reliable ML systems.

Topics include:

- Automated testing pipelines
- Deployment automation
- System health monitoring
- Alerting mechanisms
- Migration and system upgrade support

---



# Data Mining & Feature Engineering

Methods and workflows for extracting useful signals from raw data.

Topics include:

- Feature engineering pipelines
- Feature stores
- Data preprocessing
- Dataset versioning


# Git & CI/CD

Best practices for version control and continuous delivery of ML systems.

Topics include:

- Git workflows for ML projects
- CI/CD pipelines
- Automated testing
- Infrastructure and model deployment
- Environment reproducibility

# Statistics & Probability

Foundational statistical concepts required for machine learning:

- Probability distributions
- Hypothesis testing
- Statistical inference
- Sampling
- Evaluation metrics






---





### Databricks

- [The Big Book of MLOps](https://blog.infocruncher.com/resources/ml-productionisation/The%20Big%20Book%20of%20MLOps%20(Databricks,%20v6,%202022).pdf)
- [MLOps workflows on Databricks](https://docs.databricks.com/aws/en/machine-learning/mlops/mlops-workflow)
- [Model deployment patterns](https://docs.databricks.com/aws/en/machine-learning/mlops/deployment-patterns)
- [Databricks Asset Bundles resources](https://docs.databricks.com/aws/en/dev-tools/bundles/resources)
- [GenAI](GenAI-Databricks.md)

### Resources

- [Designing machine learning systems](https://github.com/chiphuyen/dmls-book/blob/main/resources.md)
- [MLOps-Tools]()
- [IEEE MLOPS](https://ieeexplore.ieee.org/document/10081336)
- [CMU Machine Learning in Production](https://ckaestne.github.io/seai/)
