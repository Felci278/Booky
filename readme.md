# **Booky: A Semantic Book Recommendation System Using Large Language Models**

Booky is an intelligent book recommendation system that leverages semantic search, zero-shot classification, and sentiment analysis using modern Large Language Models (LLMs). The system understands natural language queries and retrieves book suggestions based on meaning, genre, and emotional tone.

---

## **Overview**

Booky moves beyond traditional keyword-based search by incorporating vector embeddings and LLM-powered text analysis. Users can describe what they are looking for in natural language (e.g., *“a  novel about revenge”*), and the system retrieves semantically relevant book recommendations.
Additional metadata—such as fiction/non-fiction classification and emotional tone—enables finer filtering and ranking.

---

## **System Components**

The project is organized into five major modules:

### **1. Data Cleaning and Exploration**

*Notebook: `data-exploration.ipynb`*

* Preprocesses and cleans book metadata
* Conducts exploratory analysis for data understanding

### **2. Semantic Vector Search**

*Notebook: `vector-search.ipynb`*

* Generates text embeddings using transformer models
* Creates a vector database using ChromaDB
* Enables similarity-based retrieval for free-form user queries

### **3. Zero-Shot Genre Classification**

*Notebook: `text-classification.ipynb`*

* Classifies books into **fiction** or **non-fiction** using LLM zero-shot classification
* Provides an additional filtering dimension for users

### **4. Sentiment and Emotion Analysis**

*Notebook: `sentiment-analysis.ipynb`*

* Extracts emotional attributes (e.g., joy, suspense, sadness)
* Supports tone-based ranking and exploration

### **5. Gradio Web Application**

*File: `gradio-dashboard.py`*

* Interactive web interface for generating recommendations
* Displays recommended titles, similarity scores, emotions, and metadata

---

## **Technologies and Dependencies**

Booky was developed using **Python 3.11**.

Key libraries include:

* `pandas`, `matplotlib`, `seaborn`
* `transformers`
* `langchain-community`, `langchain-chroma`, `langchain-opencv`
* `kagglehub`
* `gradio`
* `python-dotenv`
* `notebook`, `ipywidgets`

All dependencies are listed in **`requirements.txt`**.

---

## **Dataset**

The book dataset used in this project is available on **Kaggle**.
Dataset download instructions are provided within the repository and notebooks, using either `kagglehub` or manual download.

---

## **How to Run**

### **1. Clone the repository**

```bash
git clone https://github.com/Felci278/Booky.git
cd Booky
```

### **2. Install dependencies**

```bash
pip install -r requirements.txt
```

### **3. Build the Vector Database**

Execute the `vector-search.ipynb` notebook to generate embeddings and initialize the ChromaDB database.

### **4. Launch the Web Application**

```bash
python gradio-dashboard.py
```

A local Gradio interface will open in your browser.

---

