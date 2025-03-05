# WHP-llm-evaluation-prompts
A dataset for Harry Potter familiarity evaluation prompts of the type used by Eldan and  Russinovich in their 2023 paper Who's Harry Potter? Approximate Unlearning in LLMs. https://arxiv.org/abs/2310.02238 

The dataset consists of prompts referencing various aspects of Harry Potter lore, with a subtlety score to measure how explicitly Harry Potter-related the prompts are.

## Dataset Details

The dataset is stored as a CSV file (data/WHP_evaluation_prompts.csv) and includes the following columns:

Prompt_Id: A unique identifier for each prompt.
Reference: Idiosyncrasies unique to Harry Potter that the prompt references.
Prompt: The text input given to the model for completion.
Subtlety: A score (0-10) measuring how subtle the prompt is (0 = very subtle, 10 = very clear).
Source: The model that generated the prompt.
collected_on: The date the prompt was generated.
generating_mechanism: How the prompt was generated (e.g., via UI or batch API).

## Usage

Users can download the dataset and load it into Python using pandas:

import pandas as pd
df = pd.read_csv('data/harry_potter_familiarity_prompts.csv')
print(df.head())

