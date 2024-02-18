---
title: Model Monitoring with KFServing and the Hopsworks Feature Store
publishDate: 2021-06-21 09:00:00
date: 2021-06-22 19:00:00
tags:
    - feature store
    - hopsworks
    - model monitoring
    - kfserving
    - transformer
    - online serving
category: event
keywords:
    - mlops
    - monitoring
    - feature store
    - online serving
    - feature engineering
    - streaming
draft: false
---

**Event:** [WEBINAR](https://www.linkedin.com/events/modelmonitoringwithkfservingand6807591151026151424/) | **Date:**  Tuesday, June 22th 2021

# Abstract

Turn predictions logs into valuable information that improves models over time.

Online models receive prediction requests from applications and respond with predictions. Prediction requests contain valuable information that can be extracted to (1) identify online when a model is performing poorly, (2) help data scientists offline understand the performance and behavior of the models in production, (3) create new training data if the outcome of the prediction later becomes available (by combining the prediction request with the label). Model serving infrastructure needs a platform to store/analyze/query prediction requests (and outcomes). That platform needs to be able to transform the predictions/outcomes into model monitoring metrics and support interactive queries on potentially large volumes of prediction requests. 

In this webinar, we will discuss how we integrate the KubeFlow Model Serving (KFServing) with the Hopsworks Feature Store, logging prediction requests on KFServing in Kafka and processing them with Spark before storing them in the Hopsworks Feature Store for analysis.

Attend this webinar to:
- Learn what a feature store is and how it can improve your models over time
- Learn how to recycle predictions logs and turn them into valuable information
- Watch a live demo from raw data to models in the Hopsworks Feature Store
