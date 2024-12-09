# **Advent of Haystack**

This project highlights the capabilities of [Haystack](https://github.com/deepset-ai/haystack) in solving real-world problems through a set of ten unique challenges. Developed by [*deepset*](https://www.deepset.ai/), Haystack is a robust framework for building pipelines that integrate retrieval-augmented generation (RAG), metadata processing, and other advanced NLP techniques. The event takes place during December 2024, blending technical problem-solving with a festive theme.

https://haystack.deepset.ai

> [!NOTE]  
> This project is currently WIP as not all daily challenges have not been published yet.

## **Project Description**

This project is a series of ten challenges designed to explore and enhance skills in using the Haystack framework for building advanced pipelines. Each challenge presents a scenario requiring the design, implementation, and optimization of pipelines using Haystack's tools and capabilities. The tasks focus on leveraging components from HayStack to solve practical problems.

In addition to showcasing Haystack's features, the challenges explore its application in realistic environments, working with technologies such as [Weaviate](https://weaviate.io/), [AssemblyAI](https://www.assemblyai.com/), [NVIDIA](https://www.nvidia.com/en-us/ai/), [Arize](https://arize.com/), and [MongoDB](https://www.mongodb.com/), demonstrating how Haystack integrates seamlessly with these systems to create powerful, end-to-end solutions for information retrieval and natural language processing tasks.

## **Challenges**

### **Project 1: Fetching Knowledge**
The first challenge involved building a pipeline capable of fetching content from URLs, processing it for relevance, and enabling a seamless Q&A system. The objective was to configure the pipeline to identify the ten most relevant chunks of information from the content and ensure efficient query handling.

[Notebook](./01_Enhancing_Pipeline.ipynb)

### **Project 2: Creating a RAG Pipeline and Filter Information using Weaviate**
This challenge focuses on utilizing the integration Weaviate, a vector database optimized for semantic search, to solve a fictional mystery. Goal is to design and implement a pipeline using Haystack and Weaviate that enables efficient retrieval of relevant information from a dataset answering the key question of the mystery.

[Notebook](./02_Weaviate.ipynb)

### **Project 3: Enhancing Retrieval with Multi-Query RAG**
This task focused on creating a Retrieval-Augmented Generation (RAG) pipeline that integrates multi-query retrieval techniques. The goal was to improve recall by retrieving highly relevant answers from external data sources, such as news feeds. Custom components were implemented to enhance the pipeline's performance.

[Notebook](./03_Multi_Query_Retrieval.ipynb)

### **Project 4:  Transcribing, Summarizing, and Rewriting using AssemblyAI**
This challenge focuses on combining the capabilities of Haystack with AssemblyAI to process audio data and transform it into meaningful text outputs. The goal is to build a pipeline that can handle the following tasks: transcribing an audio file into text, summarizing the content for simplicity, and rewriting it in a creative style tailored for a specific audience.

[Notebook](./04_AssemblyAI.ipynb)

### **Project 5: ...**
...

### **Project 6: ...**
...

### **Project 7: ...**
...

### **Project 8: ...**
...

### **Project 9: ...**
...

### **Project 10: ...**
...

## Setting Up the Project Environment on Windows or Linux

Follow these steps to set up the project environment with Python and necessary tools:

### **1. Install Python 3.11 with Anaconda**
- Download the Anaconda installer from the official Anaconda website.
- Install Anaconda following the graphical or command-line instructions for your operating system and add it to the PATH.
- Verify the installation by running the following commands in the terminal (Linux/macOS) or Anaconda Prompt (Windows):

  ```bash
  python --version
  ```

### **2. Create and Activate a Conda Environment**
- Create a new Conda environment named `haystack` with Python (verified for version 3.11):

  ```bash
  conda create --n haystack python=3.11
  ```

- Activate the environment:

  ```bash
  conda activate haystack
  ```

### **3. Install PyTorch with CUDA Support**
- Ensure you have a CUDA-compatible device if using GPU acceleration.
- Install PyTorch with CUDA (verified for version 12.1) support using pip:

  ```bash
  pip install torch --index-url https://download.pytorch.org/whl/cu121
  ```

### **4. Install Jupyter Notebook Support for VS Code**
- Install the necessary packages to work with Jupyter notebooks in Visual Studio Code:

  ```bash
  pip install notebook jupyterlab ipykernel
  ```

- If you haven't already, install the Jupyter extension in Visual Studio Code from the Extensions Marketplace.

### **5. Install Additional Dependencies**
- Install the additional dependencies listed in a `requirements.txt` file by running:

  ```bash
  pip install -r requirements.txt
  ```

- The `requirements.txt` file will download the latest versions of the defined packages. Please note that this project has used `haystack-ai` package version 2.8.0 and functionalities might (have) change(d) over time.
- After installing packages. open Visual Studio Code, select your Conda environment as the interpreter (*Python: Select Interpreter* from the Command Palette).
- Open the Jupyter notebook corresponding to the specific project.

### **6. Save Your OpenAI Secret Key**
- To use OpenAI's API, you need to save your secret key securely in a configuration file.
- Create a `config.json` file in your project directory and add the following content:

  ```json
  "sk-proj-...."
  ```

- Replace `"sk-proj-...."` with your actual OpenAI secret key, but make sure it is contained in the string `"..."`
- Ensure this file is not shared or pushed to version control systems like Git by adding it to `.gitignore`.

#### **7. Verify Setup**
- Open Visual Studio Code, select your Conda environment as the interpreter (*Python: Select Interpreter* from the Command Palette).
- Open the Jupyter notebook corresponding to the specific project.
