---
title: 'Build a personalized Bitcoin (BTC) virtual assistant in Python with Hopsworks and LLM function calling'
publishDate: 2024-04-18 00:00:00
date: 2024-04-23T10:30:00+01:00
tags:
    - llm
    - rag
    - function-calling
    - hopsworks
    - feature-store
    - cryptocurrencies
category: event
keywords:
    - llm
    - function-calling
    - hopsworks
draft: false
---

**Event:** [PyConDE & PyData Berlin](https://2024.pycon.de/) | **Date:**  Tuesday, April 23th 2024

**Talk:** [Link](https://pretalx.com/pyconde-pydata-2024/talk/JRRET3)

# Abstract

The human ambitious desire to get rich without effort has been a major driving force
behind the popularity of cryptocurrencies like Bitcoin and Ethereum. However, their high
volatility makes them too unpredictable, and keeping track of our investment gains and
losses over time can be tedious, if not boring.

In this talk, we will define the different components necessary to build a personalized
Bitcoin (BTC) virtual assistant in Python. The assistant will help you analyze your
transaction history, estimate future BTC prices, and calculate the future value of your
holdings based on these predictions. It will be powered by LLMs and will make use of a
recent technique called Function Calling to recognize the user intent from the
conversation history.

The ML system will be built in Python, following the best practices of the FTI
(feature/training/inference) pipeline architecture, on top of the open-source Hopsworks
platform which will provide the necessary ML infrastructure such as a feature store,
model serving, and a model registry.
