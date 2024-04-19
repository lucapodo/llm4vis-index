# LLM4Vis index

* [LLM4VIS Introduction](#llm4vis-introduction) 📝
* [LLM4VIS: Difference between the Two Approaches with and without the Wrapper](#llm4vis-difference-between-the-two-approaches-with-and-without-the-wrapper) 🔄
* [LLM4VIS hypercube](#llm4vis-hypercube) 📊
* [LLM4VIS index contents](#llm4vis-index-contents) 📚
    * [Tools](#tools) 🔧
    * [Research Paper](#research-paper) 📄
    * [Models](#models) 🤖
    * [Framework](#framework) 🛠️
    * [Dataset](#dataset) 📦
    * [Benchmark and Survey](#benchmark-and-guidance) 📈
* [Submit Your Work](#submit-your-work) 📥
* [Citation and Contribution](#citation-and-contribution) 🔖

## LLM4VIS index badge
[![Custom Badge](https://github.com/lucapodo/llm4vis-index/blob/main/badge.svg)](https://github.com/lucapodo/llm4vis-index)

## LLM4VIS Introduction

[Insert introduction to LLM4VIS here]

## Large Language Model as Data Scientists approaches: From Pure LLM strategy to hybrid one

In the realm of data science, Language Models (LMs) have emerged as powerful tools for various tasks, both as standalone entities and in conjunction with coding environments like Python. Here's a brief overview of what can be achieved using LMs in both scenarios:

- **Pure LLM Approach**: LLMs can sift through large volumes of textual data, extracting key insights, trends, and patterns without the need for additional agents or components.
- **LLMs with Code Environment Integration**: LLMs can generate code snippets for tasks like data cleaning, transformation, and normalization, which can then be executed within a coding environment to prepare data for analysis.

![Alt text](pure.svg "Pure approach")
![Alt text](hybrid.svg "Hybrid approach")

## LLM4VIS hypercube dimensions
An LLM4VIS methodology can be delineated by a hypercube comprising the following dimensions:
1. **Learning Strategy (Fine-tuning/Few-zero-shot learning)**: This dimension defines the methodology used for model training.
2. **Task-Agnosticism**: This dimension assesses whether the model's input encompasses only the dataset or incorporates user utterances.
3. **Approach**: This dimension distinguishes between a pure LLM approach and one enriched with additional tools or methodologies.
4. **Output Explainability**: This dimension determines whether the model merely provides a visualization or includes a narrative to elucidate the reasoning strategy.
5. **Effort**: This dimension quantifies the computational and strategic effort required to generate the output.

By leveraging these dimensions, it becomes feasible to categorize and evaluate all proposed approaches in the literature, providing a comprehensive overview of the current state-of-the-art in this domain.

## LLM4VIS index contents
The LLM4VIS (Language Models for Visual Information Systems) index serves as a comprehensive guide to resources, tools, research papers, models, frameworks, datasets, benchmarks, and guidance relevant to the intersection of language and visual information systems. Below is an overview of each dimension covered in the index.
- **Tools**: This section comprises essential resources like Python libraries and tools necessary to implement an effective Language Models for Visual Information Systems (LLM4Vis) approach.
- **Research Paper**: This section compiles academic papers exploring large language models applied to the data visualization field
- **Models**: This section contains all the models fine-tuned on the LLM4VIS tasks
- **Framework**: This section contains all the works focused on developing the LLM4VIS framework
- **Dataset**: This section contains a comprehensive list of all the datasets, categorized based on their task (e.g., captioning, nl2vis, ...)
- **Benchmark and Guidance**: This section contains all the research papers that provide guidelines or benchmarks for the other researchers.

### Tools
| Name | Description | 
| ----------------- | ----------- |
| [PandasAI](https://github.com/Sinaptik-AI/pandas-ai) | PandasAI is a Python library that makes it easy to ask questions to your data (CSV, XLSX, PostgreSQL, MySQL, BigQuery, Databrick, Snowflake, etc.) in natural language. Beyond querying, PandasAI offers functionalities to visualize data through graphs, cleanse datasets by addressing missing values, and enhance data quality through feature generation, making it a comprehensive tool for data scientists and analysts.
| [VannaAI](https://github.com/vanna-ai/vanna) | Vanna is an MIT-licensed open-source Python RAG (Retrieval-Augmented Generation) framework for SQL generation and related functionality. It also allows to generate visualization with plotly based on the SQL queries. | 
| [OpenAI Codeinterpreter](https://platform.openai.com/docs/assistants/tools/code-interpreter#:~:text=Code%20Interpreter%20allows%20your%20Assistant,until%20the%20code%20execution%20succeeds.) | Code Interpreter can run code iteratively to solve more challenging code, math, and data analysis problems| 


### Research Paper
| Name | Description |
| ----------------- | ----------- |
| Example1 | Description of Example1 |
| Example2 | Description of Example2 |
| Example3 | Description of Example3 |

### Models
| Name | Description |
| ----------------- | ----------- |
| Example1 | Description of Example1 |
| Example2 | Description of Example2 |
| Example3 | Description of Example3 |

### Frameworks
| Name | Description | 
| ----------------- | ----------- |
| Example1 | Description of Example1 |
| Example2 | Description of Example2 |
| Example3 | Description of Example3 |

### Datasets
| Name | Description | Task |
| ----------------- | ----------- | ------- |
| Example1 | Description of Example1 | Captioning |
| Example2 | Description of Example2 | Nl2vis |
| Example3 | Description of Example3 | Nl2vis |

### Benchmarks and Survey
| Name | Description | 
| ----------------- | ----------- | 
| [LLM4VIS evaluation](https://arxiv.org/pdf/2401.11255.pdf) | Description of Example1 |
| [Leveraging Large Models for Crafting Narrative Visualization](https://arxiv.org/pdf/2401.14010.pdf) | A survey of 79 papers to explore the role of large models in automating narrative visualization creation | 
| Example3 | Description of Example3 | 

## Submit Your Work

If you would like your work to be indexed in this repository, please submit it to us by clicking the button below.
[Submit Your Work](#) [![Submit](https://img.shields.io/badge/Submit-Your_Work-green)](#) 

## Citation and Contribution

To cite this repository in publications, please use the following Bibtex entry:
```bibtex
@misc{llm4vis_repository,
  author       = {Luca Podo, Shani Spivak},
  title        = {LLM4VIS Repository},
  year         = {2024},
  publisher    = {GitHub},
  journal      = {GitHub Repository},
  howpublished = {\url{https://github.com/lucapodo/llm4vis-index}},
}
