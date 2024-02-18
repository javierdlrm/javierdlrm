---
title: KFServing, Model Monitoring with Apache Spark and a Feature Store
publishDate: 2021-04-18 09:00:00
date: 2021-05-26 18:30:00
tags:
    - feature store
    - hopsworks
    - model monitoring
    - spark
    - kfserving
    - online serving
category: event
keywords:
    - mlops
    - monitoring
    - feature store
    - online serving
draft: false
---

**Event:** [DATA+AI SUMMIT 2021](https://databricks.com/session_na21/kfserving-model-monitoring-with-apache-spark-and-a-feature-store) | **Date:**  Wednesday, May 26th 2021

**Track:** [Open Source Data and ML Tools](https://databricks.com/dataaisummit/north-america-2021/agenda)

# Abstract

In recent years, MLOps has emerged to bring DevOps processes to the machine learning (ML) development process, aiming at more automation in the execution of repetitive tasks and at smoother interoperability between tools. Among the different stages in the ML lifecycle, model monitoring involves the supervision of model performance over time, involving the combination of techniques in four categories: outlier detection, data drift detection, explainability and adversarial attacks. Most existing model monitoring tools follow a scheduled batch processing approach or analyse model performance using isolated subsets of the inference data. However, for the continuous monitoring of models, stream processing platforms show several advantages, including support for continuous data analytics, scalable processing of large amounts of data and first-class support for window-based aggregations useful for concept drift detection.

In this talk, we present an open-source platform for serving and monitoring models at scale based on Kubeflow’s model serving framework, KFServing, the Hopsworks Online Feature Store for enriching feature vectors with transformer in KFServing, and Spark and Spark Streaming as general purpose frameworks for monitoring models in production.

We also show how Spark Streaming can use the Hopsworks Feature Store to implement continuous data drift detection, where the Feature Store provides statistics on the distribution of feature values in training, and Spark Streaming computes the statistics on live traffic to the model, alerting if the live traffic differs significantly from the training data. We will include a live demonstration of the platform in action.
