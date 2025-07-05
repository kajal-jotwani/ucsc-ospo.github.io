---
title: "LLMSeqRec: LLM Enhanced Contextual Sequential Recommender"
authors: [Connor,LinseyPang,bindong]
author_notes: ["Salesforce","Research Scientist, Lawrence Berkeley Lab"]
tags: ["osre25", "uc", "AI", "LLM", "Recommender"]
date: 2025-02-06T10:15:56-07:00
lastmod: 2025-02-06T10:15:56-07:00
---

###  Project Description
Sequential Recommender Systems are widely used in scientific and business applications to analyze and predict patterns over time. In biology and ecology, they help track species behavior by suggesting related research on migration patterns and environmental changes. Medical applications include personalized treatment recommendations based on patient history and predicting disease progression. In physics and engineering, these systems optimize experimental setups by suggesting relevant past experiments or simulations. Environmental and climate science applications include forecasting climate trends and recommending datasets for monitoring deforestation or pollution. In business and e-commerce, sequential recommenders enhance user experiences by predicting consumer behavior, suggesting personalized products, and optimizing marketing strategies based on browsing and purchase history. By leveraging sequential dependencies, these recommender systems enhance research efficiency, knowledge discovery, and business decision-making across various domains. Traditional sequential recommendation systems rely on historical user interactions to predict future preferences, but they often struggle with capturing complex contextual dependencies and adapting to dynamic user behaviors. Existing models primarily use predefined embeddings and handcrafted features, limiting their ability to generalize across diverse recommendation scenarios. To address these challenges, we propose LLM Enhanced Contextual Sequential Recommender (LLMSeqRec), which leverages Large Language Models (LLMs) to enrich sequential recommendations with deep contextual understanding and adaptive reasoning.
By integrating LLM-generated embeddings and contextual representations, LLMSeqRec enhances user intent modeling, cold-start recommendations, and long-range dependencies in sequential data. Unlike traditional models that rely solely on structured interaction logs, LLMSeqRec dynamically interprets and augments sequences with semantic context, leading to more accurate and personalized recommendations. This fusion of LLM intelligence with sequential modeling enables a more scalable, adaptable, and explainable recommender system, bridging the gap between traditional sequence-based approaches and advanced AI-driven recommendations. 



### Project Objectives
Aligned with the vision of the 2025 Open Source Research Experience (OSRE),  this project aims to develop an LLM-Enhanced Contextual Sequential Recommender (LLMSeqRec) to improve sequential recommendation accuracy across various scientific and business applications. Sequential recommender systems are widely used to analyze and predict patterns over time, assisting in fields such as biology, ecology, medicine, physics, engineering, environmental science, and e-commerce. However, traditional models often struggle with capturing complex contextual dependencies and adapting to dynamic user behaviors, as they primarily rely on vanilla sequential Id orders.
To address these limitations, this project will leverage Large Language Models (LLMs) to enhance context-aware sequential recommendations by dynamically integrating LLM-generated embeddings and contextual representations. The core challenge lies in designing LLMSeqRec, a unified and scalable model capable of enriching user intent modeling, mitigating cold-start issues, and capturing long-range dependencies within sequential data. Unlike conventional systems that rely solely on structured interaction logs, LLMSeqRec will interpret and augment sequences with semantic context, resulting in more accurate, adaptable, and explainable recommendations. Below is an outline of the methodologies and models that will be developed in this project: 

- **Step 1: Data Preprocessing & Feature Creation**: 
Develop a data processing pipeline to parse user’s sequential interaction behaviors into sequential data points for LLM-based embeddings and contextual sequential transformer modeling; Extract user behavior sequences, items’ metadata, and temporal patterns to create context-aware sequential representations for training, validation and testing; The data source can be from Amazon open public data or Movie Lense data set. The data points creation can follow SASRec (in the reference 1). 


- **Step 2: Model Development**: 
Design and implement LLM-enhanced sequential recommendation models, integrating pretrained language models to augment user-item interactions with semantic context; Develop an adaptive mechanism to incorporate external contextual signals, such as product descriptions, reviews into the sequential recommendation process; The baseline model can be SASRec pytorch implementation. 


- **Step 3: Evaluation**: :
Benchmark LLMSeqRec against state-of-the-art sequential recommenders, evaluating on accuracy, NDCG and cold-start performance; Conduct ablation studies to analyze the impact of LLM-generated embeddings on recommendation quality; Optimize model inference speed and efficiency for real-time recommendation scenarios.



### Project Deliverables
This project will deliver three components, software, model training, validation and performance evaluation and demo. The software which implements the above LLMSeqRec model will be hosted on the github repo as open-access repositories. The evaluation results and demo will be published along the  github repo .

### LLMSeqRec

- **Topics**:  LLM Enhanced Contextual Sequential Recommender
- **Skills**: Proficiency in Python, Pytorch, Github, Self-attention, Transformer
- **Difficulty**: Difficult
- **Size**: Large (350 hours)
- **Mentor**: {{% mention LinseyPang %}}, {{% mention bindong %}}

### References: 

- Self-Attentive Sequential Recommendation (SASRec)
- BERT4Rec: Sequential Recommendation with Bidirectional Encoder Representations from Transformer
- Retrieval-Augmented Generation for Knowledge-Intensive NLP Tasks
- Amazon Dataset: https://cseweb.ucsd.edu/~jmcauley/datasets.html#amazon_reviews 
- Movie Lense Data:  https://grouplens.org/datasets/movielens/  

## Introduction

I'm Connor, a student at NYU studying CS and Math. This summer I've gotten the opportunity to work on LLMSeqRec under Dr. Bin Dong and Dr. Linsey Pang. 

In today’s digital age, sequential recommender systems power everything from e-commerce suggestions to personalized content everywhere. However, traditional models fall short in capturing user intent, adapting to dynamic behavior, or tackling cold-start problems. That’s where LLMSeqRec comes in.

## Problem Statement

Most sequential recommender systems rely heavily on historical user-item interactions and predefined embeddings. This approach limits their ability to understand nuanced user preferences, struggles to scale across domains, and performs poorly in scenarios like new users or sparse data. The absence of semantic and contextual modeling is a major gap in current solutions.

## Overview of project

LLMSeqRec is a novel, LLM-enhanced sequential recommender framework that bridges this gap. By leveraging large language models (LLMs), it incorporates semantic embeddings and prompt-based contextual modeling to understand both user behavior and item metadata at a deeper level. The system explores two core approaches:

- Embedding-based: LLMs generate embeddings from item attributes.
- Prompt-based: LLMs receive full transaction history in natural language format and infer recommendations.

These techniques are tested using well-known datasets (e.g., Amazon, MovieLens), and evaluated with ranking metrics like NDCG@10 and Hit@10. The goal: deliver more accurate, context-rich, and explainable recommendations.

## Next Steps

The project is currently progressing through stages including model training, embedding integration, and evaluation. Upcoming tasks include:
- Fine-tuning enhanced models
- Designing zero-/few-shot prompts
- Running comparative experiments
- Publishing findings and writing technical blogs

As part of the [LLMSeqRec](/project/osre25/sf/LLMSeqRec) my [proposal](https://drive.google.com/file/d/1cs9lsjacSJUbXWzTfcHIukfKFwKJjUZF/view?usp=sharing) under the mentorship of Dr. Bin Dong and Dr. Linsey Pang.