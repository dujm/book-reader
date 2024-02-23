Book Reader
==============================

Build a book reader (Q&A LLM chain)

<br>

<details>
  <summary> <h2> Books</h2> </summary>
  <li> Time Machine by H. G. Wells
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



#### 1. Download this repo
```bash
git clone https://github.com/dujm/book-reader.git
```
#### 2. Create a conda environment
```bash
# create an env (here I name it "llm") with a stable Python version (e.g. Python 3.8) 
conda create -n ll python=3.11

# activate env
conda activate llm
```
#### 3. Install Python packages
```python
pip install -r ./config/requirements.txt
```

#### 4. Install jupyterlab (if you want to use it)
```bash
conda install -c conda-forge jupyterlab

# add conda environment to jupyter lab
conda install ipykernel
ipython kernel install --user --name=llm

# open jupyter lab
jupyter lab
```

#### 5. Download Ollama (optional)
 * Ollama is used in `notebooks/01-book-time-machine-llama2_7B.ipynb`
 * [Download file from Ollama website](https://ollama.ai/download)
   * Open Ollama app if you use a Mac
 * Select a model from [Model library](https://github.com/ollama/ollama).
 * Here I select llama2

```sh
# run llama2 model
ollama run llama2

# Note: when you run the model llama2 for the first time, the model is not yet downloaded. Therefore, ollama will pull the model from the Ollama website first, before it runs the model. This may take a while.
```

</details>

<br>

<details>
  <summary> <h2> Tools that I used</h2> </summary>

 * [Chroma vector database](https://github.com/chroma-core/chroma)
 * [HuggingFacePipeline](https://python.langchain.com/docs/integrations/llms/huggingface_pipelines)
 * [Langchain](https://github.com/langchain-ai/langchain)
 * [Ollama](https://github.com/ollama/ollama)
 * [SentenceTransformers](https://github.com/UKPLab/sentence-transformers)
</details>

<br>

 <details>
  <summary> <h2> Thanks to</h2> </summary>

 * [Project Gutenberg](https://www.gutenberg.org/)
 * [Databricks](https://www.edx.org/learn/computer-science/databricks-large-language-models-application-through-production)
</details>

<br>

---
<br>

#### [Go to Top](#TOP)