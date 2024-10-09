---
title: 'Build a personalized Commute virtual assistant in Python with Hopsworks and LLM Function Calling'
publishDate: 2024-10-09 00:00:00
date: 2024-09-19T15:35:00+01:00
tags:
    - llm
    - rag
    - function-calling
    - hopsworks
    - feature-store
category: event
keywords:
    - llm
    - function-calling
    - hopsworks
draft: false
---

**Event:** [PyData Amsterdam](https://amsterdam.pydata.org/) | **Date:**  Thursday, September 19th 2024

**Talk:** [Link](https://amsterdam2024.pydata.org/cfp/talk/3CJ8AN/)

# Abstract

The invention of the clock and the organization of time in zones have helped synchronize human activities across the globe. While timekeepers are better at planning and sticking to the plan, time optimists somehow believe that time is malleable and extends the closer the deadline. Nevertheless, whether you are an organized timekeeper or a creative timebender, external factors can affect your commute.

In this talk, we will define the different components necessary to build a personalized commute virtual assistant in Python. The assistant will help you analyze your historical lateness records, estimate future delays, and suggest the best time to leave home based on these predictions. It will be powered by a LLM and will use a technique called Function Calling to recognize the user intent from the conversation history.

The ML system will be built in Python, following the best practices of the FTI (feature/training/inference) pipeline architecture, on top of the open-source Hopsworks platform, which will provide the necessary ML infrastructure, such as a feature store, model serving, and a model registry.