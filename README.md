# Offensive Language Identification Dataset — EDA
This repository contains exploratory data analysis (EDA) performed on the OLID (Offensive Language Identification Dataset).
The dataset was introduced in the SemEval: Identifying and Categorizing Offensive Language in Social Media (OffensEval).
# Dataset Format
The main dataset file is:
    ***olid-training-v1.0.tsv***
    It is a tab-separated values (TSV) file with the following columns:
    | Column         | Description                                                                                                                                   |
    | -------------- | --------------------------------------------------------------------------------------------------------------------------------------------- |
    | **id**         | Unique identifier for each tweet                                                                                                              |
    | **tweet**      | The tweet text (raw text data to be analyzed)                                                                                                 |
    | **subtask\_a** | Label for **Task A**: Offensive language detection (values: `OFF` for offensive, `NOT` for not offensive)                                     |
    | **subtask\_b** | Label for **Task B**: Offensive language categorization (values: `TIN` = targeted insult, `UNT` = untargeted insult, `NULL` if not offensive) |
    | **subtask\_c** | Label for **Task C**: Target identification (values: `IND` = individual, `GRP` = group, `OTH` = other, `NULL` if not offensive)               |
# EDA Notebook
  The Jupyter notebook olid_eda.ipynb performs several exploratory analyses, including:

Checking for missing/null values

Distribution of tweet lengths (characters & words)

Most frequent hashtags and mentions

Common words, bigrams, and trigrams

Emoji usage frequency

Label distribution for subtask_a, subtask_b, and subtask_c

(Optional) Time-series visualization if datetime columns are available

# Requirements
  Install the required libraries before running the notebook:
  pip install pandas matplotlib

# Running the EDA
  Open the notebook and run all cells:
  ***jupyter notebook olid_eda.ipynb***
  This will generate plots for better understanding of the dataset and its structure.
