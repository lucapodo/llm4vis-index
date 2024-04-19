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
To link the repository to your work add the following badge: 
![Static Badge](https://img.shields.io/badge/indexed_on-llm4vis_index-red?link=https%3A%2F%2Fgithub.com%2Flucapodo%2Fllm4vis-index)

## LLM4VIS Introduction

Following the disruptive use of generative artificial intelligence across application domains, LLM4VIS (Large Language Model for Visualizations) is becoming one of the most promising research areas to advance existing NL2VIS approaches. LLM4VIS aims to use cutting-edge LLM technology to query data sources using only natural language queries and translate them into visualizations that accurately represent the underlying data. Although LLM like Llama or GPT, have shown a more advanced semantic understanding of free text, they suffer from the lack of interpretability of the model’s responses. Furthermore LLM, those involving computationally intensive and expensive architectures containing billions, and recently trillions of parameters, also have other contraindications, such as hallucinations, the lack of controllability and interpretability, and the high computational cost, hindering their large-scale adoption in applications. In particular, controllability has a notable, and often neglected, impact on applications: if a certain model is based on the adaptation of a proprietary LLM, such as GPT, the evolution of the original LLM could significantly impact the adapted model. This means that developers of a model based on a proprietary LLM do not have full control of their system.

This repository is dedicated to offering the latest advancements in this emerging field, serving as an updated resource for the community to enhance their research endeavors. We are committed to regularly updating and maintaining this repository to ensure accessibility to state-of-the-art knowledge

## Large Language Model as Data Scientists approaches: From Pure LLM strategy to hybrid one

In the realm of data science, Language Models (LMs) have emerged as powerful tools for various tasks, both as standalone entities and in conjunction with coding environments like Python. Here's a brief overview of what can be achieved using LMs in both scenarios:

- **Pure LLM Approach**: LLMs can sift through large volumes of textual data, extracting key insights, trends, and patterns without the need for additional agents or components.
- **LLMs with Code Environment Integration**: LLMs can generate code snippets for tasks like data cleaning, transformation, and normalization, which can then be executed within a coding environment to prepare data for analysis.

![Alt text](pure.svg "Pure approach")
![Alt text](hybrid.svg "Hybrid approach")

## LLM4VIS hypercube dimensions
An LLM4VIS methodology can be delineated by a hypercube comprising the following dimensions:
1. **📚 Learning Strategy (Fine-tuning/Few-zero-shot learning)**: This dimension defines the methodology used for model training.
2. **🎯 Task-Agnosticism**: This dimension assesses whether the model's input encompasses only the dataset or incorporates user utterances.
3. **🤖 Approach**: This dimension distinguishes between a pure LLM approach and one enriched with additional tools or methodologies.
4. **🩻 Output Explainability**: This dimension determines whether the model merely provides a visualization or includes a narrative to elucidate the reasoning strategy.
5. **🧗‍♂️ Effort**: This dimension quantifies the computational and strategic effort required to generate the output.

By leveraging these dimensions, it becomes feasible to categorize and evaluate all proposed approaches in the literature, providing a comprehensive overview of the current state-of-the-art in this domain.

## LLM4VIS index contents
The LLM4VIS (Language Models for Visual Information Systems) index serves as a comprehensive guide to resources, tools, research papers, models, frameworks, datasets, benchmarks, and guidance relevant to the intersection of language and visual information systems. Below is an overview of each dimension covered in the index.
- **Tools**: This section comprises essential resources like Python libraries and tools necessary to implement an effective Language Models for Visual Information Systems (LLM4Vis) approach.
- **Research Paper**: This section compiles academic papers exploring large language models applied to the data visualization field. It aslo categorizes each research paper based on the wide task they want to achive.
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
| Name | Abstract | Type |
| ----------------- | ----------- | ----- |
| [LLM4Vis: Explainable Visualization Recommendation using ChatGPT](https://arxiv.org/pdf/2310.07652.pdf) |  LLM4Vis, a novel ChatGPT-based prompting approach to perform visualization recommendation and return human-like explanations using very few demonstration examples. The approach involves feature description, demonstration example selection, explanation generation, demonstration example construction, and inference steps. To obtain demonstration examples with high-quality explanations, the method propose a new explanation generation bootstrapping to iteratively refine generated explanations by considering the previous generation and templatebased hint. | Task agnostic VRS |
| [LIDA: A Tool for Automatic Generation of Grammar-Agnostic Visualizations and Infographics using Large Language Models](https://arxiv.org/pdf/2303.02927.pdf) | LIDA, a novel tool for generating grammar-agnostic visualizations and infographics. LIDA comprises of 4 modules - A SUMMARIZER that converts data into a rich but compact natural language summary, a GOAL EXPLORER that enumerates visualization goals given the data, a VISGENERATOR that generates, refines, executes and filters visualization code and an INFOGRAPHER module that yields data-faithful stylized graphics using IGMs. LIDA provides a python api, and a hybrid USER INTERFACE (direct manipulation and multilingual natural language) for interactive chart, infographics and data story generation. | Task agnostic VRS |
| [NL2INTERFACE: Interactive Visualization Interface Generation from Natural Language Queries](https://arxiv.org/pdf/2209.08834.pdf) |  NL2INTERFACE explores the potential of generating usable interactive multi-visualization interfaces from natural language queries. With NL2INTERFACE, users can directly write natural language queries to automatically generate a fully interactive multi-visualization interface without any extra effort of learning a tool or programming language. Furthermore, users can interact with the interfaces to easily transform data and quickly see results in the visualizations. | Text2Vis |
| [ChartGPT: Leveraging LLMs to Generate Charts from Abstract Natural Language](https://ieeexplore.ieee.org/abstract/document/10443572?casa_token=0_4_DjYe0QwAAAAA:uJcxy-Z4nHa-aWVu5pEXgt0svGsyj0PoNJjTmyGwMV5B31PYkeDfSsakqCVmWviS-TPw3NjRBw) | ChartGPT, generating charts from abstract natural language inputs. However, LLMs are struggling to address complex logic problems. To enable the model to accurately specify the complex parameters and perform operations in chart generation, the task has been decomposed into a step-by-step reasoning pipeline, so that the model only needs to reason a single and specific sub-task during each run. Moreover, LLMs are pre-trained on general datasets, which might be biased for the task of chart generation. To provide adequate visualization knowledge, a dataset has been created consisting of abstract utterances and charts and improve model performance through fine-tuning. | Text2Vis |
| [Table2Charts: Recommending Charts by Learning Shared Table Representations](https://dl.acm.org/doi/pdf/10.1145/3447548.3467279) | Table2Charts framework which learns common patterns from a large corpus of (table, charts) pairs. Based on deep Q-learning with copying mechanism and heuristic searching, Table2Charts does table-to-sequence generation, where each sequence follows a chart template.  | Text2DataAnalysis |
| [SheetCopilot: Bringing Software Productivity to the Next Level through Large Language Models](https://proceedings.neurips.cc/paper_files/paper/2023/hash/0ff30c4bf31db0119a6219e0d250e037-Abstract-Conference.html) | SheetCopilot agent takes natural language as input and control spreadsheet to fulfill the requirements. The approach proposes a set of atomic actions as an abstraction of spreadsheet software functionalities. It further designs a state machine-based task planning framework for LLMs to robustly interact with spreadsheets.  | Text2DataAnalysis |

### Models
| Name | Description |
| ----------------- | ----------- |
| [BambooLLM](https://huggingface.co/pandasai/bamboo-llm) | PandasAI supports several large language models (LLMs). LLMs are used to generate code from natural language queries. The generated code is then executed to produce the result. |
| [ChartGPT](https://huggingface.co/yuan-tian/chartgpt) | This is the model proposed to convert abstract queries on a dataset to data visualization as proposed in the original reasearch paper [ChartGPT: Leveraging LLMs to Generate Charts from Abstract Natural Language](https://ieeexplore.ieee.org/abstract/document/10443572?casa_token=0_4_DjYe0QwAAAAA:uJcxy-Z4nHa-aWVu5pEXgt0svGsyj0PoNJjTmyGwMV5B31PYkeDfSsakqCVmWviS-TPw3NjRBw) |

### Frameworks
| Name | Description | 
| ----------------- | ----------- |
| [Natural Language Dataset Generation Framework for Visualizations Powered by Large Language Models](https://arxiv.org/abs/2309.10245) | VL2NL, a Large Language Model (LLM) framework that generates rich and diverse NL datasets using only Vega-Lite specifications as input, thereby streamlining the development of Natural Language Interfaces (NLIs) for data visualization. |
| [DATATALES: Investigating the use of Large Language Models for Authoring Data-Driven Articles](https://ieeexplore.ieee.org/abstract/document/10360883) | DATATALES a prototype system that leverages a LLM to generate textual narratives accompanying a given chart. |

### Datasets
| Name | Description | Type |
| ----------------- | ----------- | ------- |
| [nvBench: Natural Language to Visualization (NL2VIS) Benchmarks](https://github.com/TsinghuaDatabaseGroup/nvBench) | nvBench is a large dataset for complex and cross-domain NL2VIS task, which covers 105 domains, supports seven common types of visualizations, and contains 25,750 (NL, VIS) pairs. This repository contains the corpus of NL2VIS, with JSON format and Vega-Lite format. | Table-Query-VegaLite |
| [VIS30K](https://visimagenavigator.github.io/getStarted.html) | VIS30K is a collection of 31,481 images including every figure and table for 30 years spanning each track of the IEEE Visualization conference series (Vis, SciVis, InfoVis, and VAST). | Table-Image |
| [VisText: A Benchmark for Semantically Rich Chart Captioning](https://github.com/mitvis/vistext) | VisText is a benchmark dataset of over 12,000 charts and semantically rich captions! In the VisText dataset, each chart is represented as its rasterized image, scene graph specification, and underlying datatable. Each chart is paired with a synthetic L1 caption that describes the chart's elemental and ecoded properties and a human-generated L2/L3 caption that describes trends and statistics about the chart. | Captioning |
| [Quda: Natural Language Queries for Visual Data Analytics](https://arxiv.org/abs/2005.03257) | Quda aims to help V-NLIs recognize analytic tasks from free-form natural language by training and evaluating cutting-edge multi-label classification models. The dataset contains 14,035 diverse user queries, and each is annotated with one or multiple analytic tasks. | Queries |

### Benchmarks and Survey
| Name | Description | 
| ----------------- | ----------- | 
| [Vi(E)va LLM! A Conceptual Stack for Evaluating and Interpreting Generative AI-based Visualizations]([https://arxiv.org/pdf/2401.14010.pdf](https://arxiv.org/abs/2402.02167)) | It proposes a theoretical evaluation stack, EvaLLM, that decomposes the evaluation effort in its atomic components, characterizes their nature, and provides an overview of how to implement and interpret them. | 
| [Visualization Generation with Large Language Models: An Evaluation]([https://arxiv.org/pdf/2401.11255.pdf](https://arxiv.org/pdf/2401.11255.pdf)) | This paper evaluates the capability of a large language model to generate visualization specifications on the task of natural language to visualization (NL2VIS). More specifically, it used GPT-3.5 and Vega-Lite to represent large language models and visualization specifications respectively. |
| [Doom or Deliciousness: Challenges and Opportunities for Visualization in the Age of Generative Models](https://onlinelibrary.wiley.com/doi/full/10.1111/cgf.14841) | This paper attempts to understand the roles that generative models might play across visualization. It does so by constructing a framework that characterizes what these technologies offer at various stages of the visualization workflow, augmented and analyzed through semi-structured interviews with 21 experts from related domains. Through this work, the authors map the space of opportunities and risks that might arise in this intersection, identifying doomsday prophecies and delicious low-hanging fruits that are ripe for research. | 
| [Are LLMs ready for Visualization?](https://arxiv.org/pdf/2403.06158.pdf) | The paper goal is to propose a systematic approach that analyzes three elements: whether Large Language Models are capable of correctly generating a large variety of charts, what libraries they can deal with effectively, and how far we can go to configure individual charts. To achieve this objective, the authors initially selected a diverse set of charts, which are commonly utilized in data visualization.| 

## Submit Your Work

If you would like your work to be indexed in this repository, please submit it to us by clicking the button below.
[![Submit](https://img.shields.io/badge/Submit-Your_Work-green)](https://forms.gle/iV6wxR8wFoFvqowk8) 

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
