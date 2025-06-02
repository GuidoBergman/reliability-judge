# Reliability Judge: Enhancing LLM Reliability Through Multi-Model Judging

## Abstract

We present a multi-model judging framework that extends the Think Twice before Trusting (T3) paradigm to enhance answer reliability across large language models (LLMs). Our approach is most suitable for high-stakes contexts (e.g., healthcare, legal, or safety-critical systems), where even minor accuracy gains can have significant consequences. The proposed system uses cross-model evaluation to identify the most accurate and well-justified response from a set of candidates. Each model acts both as an answer generator and as a judge under two modes: as a neutral evaluator or as a participant evaluating its own response. Judgments consider factual correctness, reasoning clarity, and confidence-justification alignment. Our results show that the best judge-based approach outperforms all the monolithic (i.e., single-model) versions. This work contributes a transparent method for selecting high-confidence outputs from black-box models, advancing practical AI reliability and alignment.

## Project structure
- **generate_answers.ipynb**: contains the code to run all the purposed variants (monolithic, judge as participant and judge as evaluator only) against the MMLU Pro dataset and save the results in CSV files.
- **data_analysis.ipynb**: contains the code used to analyze the results including all the plots.
- **results**: folder that contains the CSV files with the results of the variants for each model.