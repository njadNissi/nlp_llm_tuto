# Introduction Tutorial for Large Language Model (Natural Language Processing)
A large language model (LLM) is a type of computational model designed for natural language processing tasks such as language generation. As language models, LLMs acquire these abilities by learning statistical relationships from vast amounts of text during a self-supervised and semi-supervised training process. The largest and most capable LLMs are artificial neural networks built with a decoder-only transformer-based architecture, enabling efficient processing and generation of large-scale text data. Modern models can be fine-tuned for specific tasks, or be guided by prompt engineering. These models acquire predictive power regarding syntax, semantics, and ontologies inherent in human language corpora, but they also inherit inaccuracies and biases present in the data on which they are trained.
**Read more on on Large Language Model [here](https://en.wikipedia.org/wiki/Large_language_model)**

## Steps
* **1. Clone or download this repo**
* **2. download the models [LLM .pth FILES](https://www.kaggle.com/models/njadnissi/llm_pth_models)	from and paste into `4_training_gpt` folder** as shown below:
```
4_training_gpt/
├── gpt2         <------------------------------------ Unzip and paste this folder in here 
│   └── 124M
│       ├── checkpoint
│       ├── encoder.json
│       ├── hparams.json
│       ├── model.ckpt.data-00000-of-00001
│       ├── model.ckpt.index
│       ├── model.ckpt.meta
│       └── vocab.bpe
├── images
│   ├── CPU_performance.png
│   └── CPU_Performance.png
├── model_and_optimizer.pth 	<--------------------- Unzip and Copy this file in here
├── model.pth	<------------------------------------- Unzip and Copy this file in here
└── training_gpt
    ├── loss-plot.pdf
    ├── model.py
    ├── openai_gpt2.py
    ├── the-verdict.txt
    ├── train_model.ipynb
    └── utils.py
```
* **3. Install an Integrated Development Environment** [PyCharm](https://www.jetbrains.com/help/pycharm/installation-guide.html), [VSCode](https://code.visualstudio.com/docs) or [any other](https://www.google.com/search?client=ubuntu-sn&channel=fs&q=python+IDEs) you prefer, then launch the IDE.
* **4.Install Virtual Environments Manager**  [Conda](https://docs.conda.io/projects/conda/en/latest/user-guide/install/index.html), [MiniConda](https://docs.anaconda.com/miniconda/install), [Anaconda](https://docs.anaconda.com/anaconda/install/) or you can just use the python inbuilt [venv](https://docs.python.org/3/tutorial/venv.html).
* **5. Move into project directory In your Terminal(inside or outside the IDE) and Run:**
	
	With **Conda**:
	```bash
	### Create Virtual Environment and Install Packages
	conda env create -f environment.yml
	### Activate:
	conda activate llm_env
	```
	
	With **venv (pip)**:
	```bash
	### Create Virtual Environment
	python3 -m venv llm_env

	### Activate:
	for linux/macos: source <path-to-llm_env>/bin/activate
	for windows Bash: cd <path-to-llm_env>\Scripts && activate

	### Install pip
	python install --upgrade pip

	###Confirm installation and pip path
	for linux/mac: which pip
	for windows: where pip
	
	### Install packages
	make sure you are in the project directory: cd <path-to-llm_env>
	pip install -r requirements.txt
	```
