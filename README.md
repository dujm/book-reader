Book Reader
==============================

Build a book reader using LLM

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
    │   └── `00-book-time-machine.ipynb`: teaching LLM to read the book "Time Machine"
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