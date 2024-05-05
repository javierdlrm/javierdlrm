---
title: 'Streaming Feature Pipelines with QuixStreams for Real-Time Coinbase Market AI'
publishDate: 2024-04-18 00:00:00
date: 2024-04-25T17:45:00+01:00
tags:
    - streaming
    - feature-pipeline
    - hopsworks
    - feature-store
    - quixstreams
    - cryptocurrencies
category: event
keywords:
    - streaming
    - feature-pipeline
    - hopsworks
    - quixstreams
draft: false
---

**Event:** [Stream Processing Meetup at SumUp Berlin](https://www.meetup.com/en-us/berlin-stream-processing-meetup-group/events/300070091/) | **Date:**  Thursday, April 25th 2024

**Hosted by:** Quix.io

# Abstract

In this talk, we will build a streaming feature pipeline that consumes real-time orderbook events from the Coinbase APIs and outputs curated ML features that can be used to build a prediction service.
First, we will use QuixStreams to process the raw events, compute time-windowed aggregations and deliver the curated ML features to Kafka, from where they will be ingested into the Hopsworks Feature Store.