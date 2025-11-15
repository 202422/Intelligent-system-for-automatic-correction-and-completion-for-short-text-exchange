# Intelligent-system-for-automatic-correction-and-completion-for-short-text-exchange

## Context
**Short Texts often contain:**

- Typos and spelling errors.
- Incomplete or ambiguous sentences.


**The objective is to create a system capable of:**

- Automatically correcting spelling and grammatical errors.
- Completing or suggesting the continuation of incomplete text.


## Data Source


The dataset used in this project comes from the **First Certificate in English (FCE) dataset**, which is part of the **Cambridge Learner Corpus (CLC)** released by the **University of Cambridge**. It contains exam scripts written by English learners. Each document is annotated with information about grammatical, lexical, and mechanical errors, along with the corrected versions provided by expert annotators. The dataset is organized into folders containing XML files, where each file represents an individual learner’s essay, including metadata about the task, learner proficiency level, and error annotations.


To collect the dataset named *automatic_correction_dataset.csv*, I have created a script that:

- Traverses all subfolders and XML files
- Extracts only \<p> paragraphs with \<NS>\<i>\</i>\<c>\</c>\</NS>
- Splits into sentences, extract wrong/correct pairs
- Aggregates all pairs in a DataFrame

## Auto correcteur

![](/Assets/metric.png)  

![](/Assets/test.png)
