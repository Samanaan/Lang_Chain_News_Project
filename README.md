![Python](https://img.shields.io/badge/python-3.9-blue)
![LangChain](https://img.shields.io/badge/langchain-active-brightgreen)
![OpenAI](https://img.shields.io/badge/OpenAI-GPT--4-orange)

## 📰 News Query Assistant

A custom knowledge assistant that answers news-related questions by combining OpenAI, LangChain, and a vector database (Chroma).
Unlike a pure LLM baseline, this pipeline grounds answers in real documents, fact-checks outputs, and evaluates correctness against retrieved sources.

---

## ✨ Features

🔍 Retrieval-Augmented Generation (RAG): Retrieves relevant passages from AG News and BBC datasets.

✅ Fact-Checking Stage: Ensures answers are grounded in retrieved evidence.

📑 Inline Citations: Answers are annotated with [Source-X] style references.

⚖️ Evaluation Pipeline: Compares pipeline vs baseline answers and judges correctness.

🛠 Modular Design: Swap in different datasets or vector stores with minimal changes.

---

## 📂 Project Structure

├── News_query_project.ipynb   # Main notebook with pipeline

├── data/                      # Placeholder for datasets (AG News, BBC, etc.)

├── images/                    # Screenshots / diagrams for README

├── requirements.txt           # Dependencies

└── README.md                  # Project overview

---

## 🚀 Usage

Run the Jupyter Notebook step by step:

1. Load datasets (AG News + BBC latest).

2. Create vector store using Chroma and OpenAI embeddings.

3. Run pipeline with:

  - Draft answer generation

  - Fact-checking

  - Final answer with citations

4. Evaluate pipeline vs baseline to measure accuracy improvements.

---

## 📊 Example Output

Evaluation Table

![alt text](https://github.com/images/2025-09-15 at 12.47.28 AM.png)

Pipeline Architecture

"Include a diagram (can make a simple flowchart in draw.io or Excalidraw):"

---

## 🧪 Sample Questions

Who is the CEO of Microsoft?

What are the latest trends in renewable energy?

What happened in the 2008 financial crisis?

Who won the 2016 U.S. presidential election?

What is quantum computing?

---

## 🔮 Future Improvements

Add weighted retriever to prioritize fresher sources.

Integrate live news APIs (e.g., NewsAPI, GDELT) instead of static datasets.

Deploy as a web app with Streamlit or FastAPI.

Expand evaluation with LLM-as-judge + human spot-checks.
