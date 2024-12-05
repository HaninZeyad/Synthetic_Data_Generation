## Data Generation Methods
I examined two data generation methods:

### Method 1: Instruction-based Data Generation with txtinstruct

I used txtinstruct, a framework designed for training models on instruction-based tasks.
The data was curated using a question generation model based on the SQuAD dataset. This model generates various types of questions (e.g., Who/What/When/Where/How) and declarative prompts like "Tell me about," "Describe the," and "Explain how."
FLAN-T5 was used as the language model to generate target statements, followed by a fine-tuning process with the google/flan-t5-small transformer model.
The resulting dataset was integrated into the txtai pipeline for further use in model training.


### Method 2: Open-Chat (Synthetic Data Generation)

For this method, synthetic data was generated using large language models (LLMs), specifically leveraging their ability to create a wide variety of task-specific prompts and labeled examples for model tuning.
The synthetic data generated was used to fine-tune models for various instruction-based tasks, improving their performance on downstream tasks# Synthetic_Data_Generation
