Book Reader
==============================

Build a book reader (Q&A LLM chain)

<br>

Books 
--------------------
 * Time Machine by H. G. Wells

<br>

Project Organization
--------------------
    .
    ├── AUTHORS.md
    ├── LICENSE
    ├── README.md
    ├── config
    │   ├── `requirements.txt`: packages
    │   └── `token_access.py`: the file is used to store tokens (remember to add the filename in `.gitignore` file to protect your token) 
    ├── data
    ├── notebooks
    │   ├── `00-book-time-machine_flan_t5_large.ipynb`: using `google/flan-t5-large`
    │   └── `01-book-time-machine-llama2_7B.ipynb`: using `llama2_7B`

    └── model
        └──cache: storing models

<br>

Tools used
--------------------
 * [Chroma vector database](https://github.com/chroma-core/chroma)
 * [HuggingFacePipeline](https://python.langchain.com/docs/integrations/llms/huggingface_pipelines)
 * [Langchain](https://github.com/langchain-ai/langchain)
 * [SentenceTransformers](https://github.com/UKPLab/sentence-transformers)


<br>

Thanks to
--------------------
 * [Project Gutenberg](https://www.gutenberg.org/)
 * [Databricks](https://www.edx.org/learn/computer-science/databricks-large-language-models-application-through-production)