---
title: Scalable Architecture for Automating Machine Learning Model Monitoring
date: 2020-07-01 00:00:00
download_link: http://kth.diva-portal.org/smash/record.jsf?pid=diva2%3A1464577&dswid=-9436
tags:
    - neurodegeneration
    - alzheimer
categories:
    - thesis
    - research
keywords:
    - neurodegeneration
    - alzheimer
    - adni
draft: false
---

### Abstract

Last years, due to the advent of more sophisticated tools for exploratory data analysis, data management, Machine Learning (ML) model training and model serving into production, the concept of MLOps has gained more popularity. As an effort to bring DevOps processes to the ML lifecycle, MLOps aims at more automation in the execution of diverse and repetitive tasks along the cycle and at smoother interoperability between teams and tools involved. In this context, the main cloud providers have built their own ML platforms [4, 34, 61], offered as services in their cloud solutions. Moreover, multiple frameworks have emerged to solve concrete problems such as data testing, data labelling, distributed training or prediction interpretability, and new monitoring approaches have been proposed [32, 33, 65]. Among all the stages in the ML lifecycle, one of the most commonly overlooked although relevant is model monitoring. Recently, cloud providers have presented their own tools to use within their platforms [4, 61] while work is ongoing to integrate existent frameworks [72] into open-source model serving solutions [38]. Most of these frameworks are either built as an extension of an existent platform (i.e lack portability), follow a scheduled batch processing approach at a minimum rate of hours, or present limitations for certain outliers and drift algorithms due to the platform architecture design in which they are integrated. In this work, a scalable automated cloudnative architecture is designed and evaluated for ML model monitoring in a streaming approach. An experimentation conducted on a 7-node cluster with 250.000 requests at different concurrency rates shows maximum latencies of 5.9, 29.92 and 30.86 seconds after request time for 75% of distance-based outliers detection, windowed statistics and distribution-based data drift detection, respectively, using windows of 15 seconds length and 6 seconds of watermark delay.

----

Under de senaste åren har konceptet MLOps blivit alltmer populärt på grund av tillkomsten av mer sofistikerade verktyg för explorativ dataanalys, datahantering, modell-träning och model serving som tjänstgör i produktion. Som ett försök att föra DevOps processer till Machine Learning (ML)-livscykeln, siktar MLOps på mer automatisering i utförandet av mångfaldiga och repetitiva uppgifter längs cykeln samt på smidigare interoperabilitet mellan team och verktyg inblandade. I det här sammanhanget har de största molnleverantörerna byggt sina egna ML-plattformar [4, 34, 61], vilka erbjuds som tjänster i deras molnlösningar. Dessutom har flera ramar tagits fram för att lösa konkreta problem såsom datatestning, datamärkning, distribuerad träning eller tolkning av förutsägelse, och nya övervakningsmetoder har föreslagits [32, 33, 65]. Av alla stadier i ML-livscykeln förbises ofta modellövervakning trots att det är relevant. På senare tid har molnleverantörer presenterat sina egna verktyg att kunna användas inom sina plattformar [4, 61] medan arbetet pågår för att integrera befintliga ramverk [72] med lösningar för modellplatformer med öppen källkod [38]. De flesta av dessa ramverk är antingen byggda som ett tillägg till en befintlig plattform (dvs. saknar portabilitet), följer en schemalagd batchbearbetningsmetod med en lägsta hastighet av ett antal timmar, eller innebär begränsningar för vissa extremvärden och drivalgoritmer på grund av plattformsarkitekturens design där de är integrerade. I det här arbetet utformas och utvärderas en skalbar automatiserad molnbaserad arkitektur för MLmodellövervakning i en streaming-metod. Ett experiment som utförts på ett 7nodskluster med 250.000 förfrågningar vid olika samtidigheter visar maximala latenser på 5,9, 29,92 respektive 30,86 sekunder efter tid för förfrågningen för 75% av avståndsbaserad detektering av extremvärden, windowed statistics och distributionsbaserad datadriftdetektering, med hjälp av windows med 15 sekunders längd och 6 sekunders fördröjning av vattenstämpel.
