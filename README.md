## Dependency Trigger NER
### Introduction

DepTrigger, a simple and effective approach in low-resource named entity recognition (NER) based on multi-hop dependency trigger.

Experiments show that using only 20% of the trigger-annotated sentences results in a comparable performance as using 70% of conventional annotated sentences.

DepTrigger refers to salient nodes relative to an entity in the dependency graph of a context sentence. We apply Stanford CoreNLP to the individual sentences to obtain dependency paths.


DepTrigger is closely related to the TriggerNER: Learning with Entity Triggers as Explanations for Named Entity Recognition.

Compared to TriggerNER, DepTrigger outperforms for long sentences, while still maintain good performance for short sentences as usual. Our framework is significantly more cost-effective in real business.


### Requirements

1. torch==1.8.1
2. scikit-learn==0.24.2

### Trigger datasets

1. trigger_20.txt: 20% original train set which include trigger-annoated sentences；
2. trigger_prim_100.txt: only primary triggers dataset；
3. trigger_sec_100.txt: only secondary triggers dataset；

### Download
word ：glove.6B.100d.txt， place it in gloveEN/。

### train

1. run supervised.py；code modified from https://github.com/INK-USC/TriggerNER

