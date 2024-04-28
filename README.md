# Amharic Llama

**Goal**: To create the best possible Amharic language models that can run offline on a budget smartphone.

All resources created from this repository will be stored in [amharic_llama](https://huggingface.co/collections/simonbutt/amharic-llama-6626f00939a93f2db639588e) huggingface collection.

Unless otherwise stated, notebooks through [Google Colab](https://colab.research.google.com/) are the primary supported way of running everything here. 

## Vision
- Create a robust evaluation framework to understand current Amharic LLM capabilities.
- Develop the SoA Amharic language models for <3B and <10B parameters.
- Develop an offline AI app to enable broad distribution for Ethiopians running on low RAM hardware.
- Progress to Oromo, Tigrinya, Afar and Somali languages. 

## Process

### Phase 1 - Evaluate 
**Objective**: Understand the current SOA in Amharic 

- [ ] Fine tune various SOA english LLMs on Amharic translated datasets to provide a set of control models.
    - [x] Alpaca - [Model](https://huggingface.co/simonbutt/am_llama3_alpaca), [Dataset](https://huggingface.co/datasets/iocuydi/amharic-alpaca)
    - OpenOrca 
    - Textbooks
- [ ] Develop an open Amharic LLM Leaderboard for model evaluation
    - Translate Evaluation Datasets - [Amharic GSM8K](https://huggingface.co/datasets/simonbutt/amharic_gsm8k), [Amharic TruthfulQA](https://huggingface.co/datasets/simonbutt/amharic_truthful_qa), ARC, HellaSwag, MMLU, Winogrande
    - Create [lm-evaluation-harness](https://github.com/EleutherAI/lm-evaluation-harness) tasks for each translated dataset
    - Create an Amharic LLM leaderboard to visualise all existing model capabilities.
    
### Phase 2 - Train
**Objective**: Use EEVE vocabulary expansion to train the SOA Amharic language model.
