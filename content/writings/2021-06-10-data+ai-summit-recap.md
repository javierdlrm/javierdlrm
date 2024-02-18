---
title: Data+AI Summit Recap - Everything that you missed on Feature Stores
date: 2021-06-10 08:00:00
tags:
    - data+ai summit
    - feature store
categories:
    - post
keywords:
    - feature engineering
    - feature store
draft: false
---

**Authors:** Davit Bzhalava, Javier de la Rúa Martínez

> *Full disclosure: Javier de la Rúa Martínez from Logical Clocks presented a talk at the summit.*

This year's Data and AI summit emphasised the Feature Store as an essential part to conduct successful ML Operations (MLOps). There were six talks that addressed this emerging technology, both from Enterprise vendors and industry-leaders. We have compiled here a summary of each presentation. We’ll include the video recordings from each session once they become available.

## Databricks unveils its Feature Store

[In the keynote session](https://dataaisummit.com/session-virtual/?v26dd132ae80017cdaf764437c30ebe6f10c1b1eeaab01165e44366654b368dfaeab6baf7e386a642ecb238989334530e=683B3F805A396FBD0F2D131CFE84E9FD4B94512D08D5572799960E61DE6F05BB58334E53D5AFEFAFC80C01338A52E263) Databricks announced the release of a Feature Store as a part of the Databricks ML ecosystem. It is accessible only in Databricks Runtime notebooks and notebook jobs. Its offline feature store is built on top of Delta Lake thus provides time travel functionalities. For online stores it uses Amazon Aurora (MySQL-compatible) and Amazon RDS MySQL databases, however online inference of models is not supported, only batch scoring is supported. Databricks' Feature Store provides full lineage capabilities to track from models to features and vica versa, as well as provides functionality to search and browse features from the UI. 

## Feature Store with KFServing for Model Serving

In the [presentation](https://databricks.com/session_na21/kfserving-model-monitoring-with-apache-spark-and-a-feature-store) by Logical Clocks, they identified the need to provide online applications using operational models with historical and context features that are not available within the application itself. The Feature Store can massively increase the power of machine learning models by making more features available in real-time, and with more features you have the potential to make more accurate predictions. They described how models are represented in the Hopsworks Feature Store using training datasets, how the Online Feature Store is powered by RonDB, the world’s most advanced open-source LATS (low-Latency, high-Availability, high-Throughput, and high-Scalability) database, how their Feature Store can be used by KFServing to enrich prediction requests with recent data on-the-fly, and finally how prediction logs can be continuously analyzed with Spark to monitor the performance of your models. Last but not least, they give an insight into unifying feature drift and data drift detection using the built-in data validation capabilities of the Hopsworks Feature Store, playing the role of an Evaluation Store.

## Humana’s Feature Store for Data Science

During this [session](https://databricks.com/session_na21/florenceai-reinventing-data-science-in-the-cloud-at-humana), Humana presented their in-house collaborative ML platform FlorenceAI. The primary goal of FlorenceAI is to automate and accelerate the management of the ML model life cycle by enabling a large number of data scientists and ML/data engineers to collaborate in a single platform. This is achieved by their feature store which is a core part of FlorenceAI. It hosts over tens of thousands of features with several years of historical data and are refreshed in a daily and monthly cadences. FlorenceAI is built on top of Azure Databricks, Delta lake, MLFlow, AppInsights and Azure Data Factory.

## Feature Store on Delta Lake

[This session](https://databricks.com/session_na21/a-practical-enterprise-feature-store-on-delta-lake), presented by Navy Federal Credit Union, outlined the scope of Feature Stores and its role to perform MLops at scale. Their in-house Feature Store helped them to accelerate data science experimentation and model deployments to production. It is built on top of Delta Lake and is based on Feast with extra capabilities, such as dynamic feature store selection tools and DSL that abstract complexity of point in time joins.

## Feature Store powered by an HTAP database

In this [session](https://databricks.com/session_na21/unified-mlops-feature-stores-model-deployment), the team behind Splice Machine emphasized the benefits of using their Hybrid Transactional/Analytical Processing (HTAP) database across the different stages of the ML lifecycle, playing the role of a Feature Store for deduplicating data pipelines, and a Deployment and Evaluation Store for serving models and monitoring their performance. They describe Splice Machine as a HTAP database built on HBase, and supporting Spark, that, in contrast with other HTAP databases, is fully ACID compliant, supports indexes and triggers, provides point-in-time consistency and can scale to any cloud and on-premises. It contains a cost-based optimizer that allows users writing SQL queries which are then compiled into binary code to run the operations. In addition, Splice Machine provides support for storing models in cache memory, making predictions and logging the prediction logs automatically at millisecond speed.
    
## Feature Store if you’re getting started

During the [session](https://databricks.com/session_na21/rethinking-feature-stores) presented by Tecton, they provided a complete overview of what a Feature Store is, revisiting the main components of their architecture and outlining the advantages of using a Feature Store in  your ML projects such as consistent feature transformations or feature validation/monitoring capabilities. They placed special emphasis on the importance of following a model-centric approach, aiming at decoupling ML applications from environment-specific infrastructure. In this context, they introduced the next release of Feast - an end-to-end open source feature store - with version 0.10 (gcp-focused) which includes new improvements to make it easier for teams to get started and deal with different environments such full support for running locally, no configuration or infrastructure required or extensibility.