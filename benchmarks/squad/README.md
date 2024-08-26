# SQuAD

[SQuAD (v1.1)](https://arxiv.org/abs/1606.05250) is a benchmark for testing machine reading comprehension and reasoning abilities, leveraging 100,000+ questions posed by crowdworkers on a collection of Wikipedia articles.

Here, we implement the evaluation for the Stanford Question Answering Dataset (SQuAD) v1.1, which is currently formulated as a single task which adopts a custom F1 and Exact Match scorer. 

The goal is to provide an answer which matches between 1 to 3 of the target answers, in response to a question based on a paragraph from a provided Wikipedia article. 

The questions are designed to vary lexically and syntactically from the provided paragraphs, and thus, answering them requires advanced reasoning capabilities.

## Execution
Here is an example from the dataset:
```
Context: 

Question: 

Answer(s): 
```
The model is tasked to answer the question by referring to the context, potentially requiring mutliple-sentence reasoning.

## Evaluation


## Note on SQuAD v2
SQuAD v2 combines the SQuAD v1.1 dataset with 50,000+ unanswerable questions, written adversarially by crowdworkers to look similar to answerable ones.

To perform well, systems must not only answer questions when possible, but also determine when no answer is supported by the paragraph and abstain from answering. 

This will be developed in a later iteration of the benchmark implementation.