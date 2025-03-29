# 📚 Build a Semantic Book Recommender with LLMs – Full Course

This repository contains all the code from the "Build a Semantic Book Recommender with LLMs – Full Course", originally published by freeCodeCamp and Jetbrains. This repo includes my adaptations and enhancements of the course. The code provided here has been adapted to ensure compatibility with my local development environment and optimize overall project performance. There are five components to this tutorial:
* Text data cleaning (code in the notebook `data-exploration.ipynb`)
* Semantic (vector) search and how to build a vector database (code in the notebook `vector-search.ipynb`). This allows users to find the most similar books to a natural language query (e.g., "a book about a person seeking revenge").
* Doing text classification using zero-shot classification in LLMs (code in the notebook `text-classification.ipynb`). This allows us to classify the books as "fiction" or "non-fiction", creating a facet that users can filter the books on. 
* Doing sentiment analysis using LLMs and extracting the emotions from text (code in the notebook `sentiment-analysis.ipynb`). This will allow users to sort books by their tone, such as how suspenseful, joyful or sad the books are.
* Creating a web application using Gradio for users to get book recommendations (code in the file `gradio-dashboard.py`).

⚙️ Customizations
Throughout the practical application of the course, I performed several customizations to the original code to ensure it would run correctly and consistently on my setup. Key adaptations include:

* Complete environment adaptation from macOS (original course setup) to Windows, including package substitutions and OS-specific compatibility fixes.

* Full support for GPU acceleration using NVIDIA CUDA.

* File encoding handling with UTF-8, addressing issues common in Windows environments.

* Updates and replacements of packages to maintain compatibility with Python 3.11.

* Modifications in notebooks and scripts to ensure smooth execution on Windows, handling encoding, terminal permissions, and other platform-specific concerns.

Additionally, a full review of the dependencies was conducted. Significant differences in package versions were found when comparing the original requirements.txt to the actual environment used for development:

* Updated packages: such as gradio, transformers, openai, langchain, and chromadb.

* New packages added: including torch, torchaudio, and torchvision with CUDA support.

* Missing dependencies from the original list, which were necessary for full functionality on Windows.

📦 Requirements

This project was initially created in Python 3.11. In order to run the project, the following dependencies are required:
* [kagglehub](https://pypi.org/project/kagglehub/)
* [pandas](https://pypi.org/project/pandas/)
* [matplotlib](https://pypi.org/project/matplotlib/)
* [seaborn](https://pypi.org/project/seaborn/)
* [python-dotenv](https://pypi.org/project/python-dotenv/)
* [langchain-community](https://pypi.org/project/langchain-community/)
* [langchain-opencv](https://pypi.org/project/langchain-opencv/)
* [langchain-chroma](https://pypi.org/project/langchain-chroma/)
* [transformers](https://pypi.org/project/transformers/)
* [gradio](https://pypi.org/project/gradio/)
* [notebook](https://pypi.org/project/notebook/)
* [ipywidgets](https://pypi.org/project/ipywidgets/)

All package versions and dependencies used in my environment are documented in requirements.txt, which should be preferred for environment replication.

🔐 API Configuration
To generate the vector database, a .env file must be created in the project root directory containing your OpenAI API key. The official tutorial explains how to obtain and configure this key.

🛢️ Dataset Source
The dataset used in this project is available on Kaggle. Instructions for downloading and preparing the data are provided in the original course repository.

This project was adapted by Neyran for educational and technical purposes.
The changes aim to improve portability, stability, and cross-platform compatibility of the original codebase.

