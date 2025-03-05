## Introduction
The **Harry Potter Familiarity Prompt Dataset** is designed to evaluate language models on their ability to recognize and respond to prompts related to the **Harry Potter** universe. Each prompt references elements of the **Harry Potter** lore with varying levels of subtlety, allowing for an assessment of how well an LLM understands both explicit and implicit references.

## Data Fields
The dataset contains the following columns:

| Column Name         | Description |
|---------------------|-------------|
| **Prompt_Id**      | A unique identifier assigned to each prompt. |
| **Reference**      | The specific **Harry Potter**-related concept referenced in the prompt (e.g., spells, character names, locations). |
| **Prompt**        | The full text of the prompt you can provide to to the model. |
| **Subtlety**       | A numerical score from **0 (very subtle)** to **10 (very clear)**, measuring how explicitly the prompt references **Harry Potter**. |
| **Source**         | The language model that generated the prompt. |
| **collected_on**   | The date when the prompt was generated and recorded. |
| **generating_mechanism** | Specifies the method used to generate the prompt (e.g., **via UI** interaction or **batch API** processing). |

## Data Collection Methodology
Prompts were gathered through interactions with multiple **LLMs**, using both **manual and automated methods**. The **subtlety score** was assigned based on how recognizable the reference was within the **Harry Potter** universe. 

## Potential Use Cases
This dataset can be utilized for:
- **Evaluating LLM familiarity** with **Harry Potter**-themed prompts.
- **Benchmarking model performance** on domain-specific knowledge.
- **Fine-tuning language models** to improve their responses to literary universe prompts.
- **Estimating unlearning effectiveness** when subjecting the model to different unlearning methodologies.
