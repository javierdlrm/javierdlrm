---
title: The Hopsworks Feature Store for Machine Learning
date: 2024-06-09 00:00:00
download_link: https://dl.acm.org/doi/10.1145/3626246.3653389
tags:
    - feature-store
    - arrow-flight
    - duckdb
    - ml-systems
categories:
    - ml-systems
    - data-management-systems
keywords:
    - feature-store
    - mlops
    - rondb
    - arrow-flight
    - duckdb
draft: false
---

[SIGMOD PODS 2024 - Industrial Track](https://2024.sigmod.org/) | **Date:**  Wednesday, June 12th 2024

### Abstract

Data management is the most challenging aspect of building Machine Learning (ML) systems. ML systems can read large volumes of historical data when training models, but inference workloads are more varied, depending on whether it is a batch or online ML system. The feature store for ML has recently emerged as a single data platform for managing ML data throughout the ML lifecycle, from feature engineering to model training to inference.
In this paper, we present the Hopsworks feature store for machine learning as a highly available platform for managing feature data with API support for columnar, row-oriented, and similarity search query workloads. We introduce and address challenges solved by the feature stores related to feature reuse, how to organize data transformations, and how to ensure correct and consistent data between feature engineering, model training, and model inference. We present the engineering challenges in building high-performance query services for a feature store and show how Hopsworks outperforms existing cloud feature stores for training and online inference query workloads.
