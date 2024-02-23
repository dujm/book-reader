Book Reader
==============================

Build a book reader (Q&A LLM chain)

<br>

<details>
  <summary> <h2> Books</h2> </summary>
  <p> 
  <li> Time Machine by H. G. Wells
  </p>
</details>

<br>


<details>
  <summary> <h2> Project Organization</h2> </summary>


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
</details>
<br>

<details>
  <summary> <h2> How to use this repo?</h2> </summary>
  <h4> Download the repo</h4>
</details>

-------------------

#### Download the repo
```bash
git clone https://github.com/dujm/book-reader.git
```
#### Create a conda environment
```bash
# create an env (here I name it "llm") with a stable Python version (e.g. Python 3.8) 
conda create -n ll python=3.11

# activate env
conda activate llm
```
#### Install Python packages
```python
pip install -r ./config/requirements.txt
```

#### Install jupyterlab (if you want to use it)
```bash
conda install -c conda-forge jupyterlab

# add conda environment to jupyter lab
conda install ipykernel
ipython kernel install --user --name=llm

# open jupyter lab
jupyter lab
```

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