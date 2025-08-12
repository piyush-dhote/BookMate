# 📚 Book Recommender System using Sentence Transformers

An intelligent book recommendation system that understands your queries using Hugging Face's `sentence-transformers` to suggest semantically and emotionally relevant books. Unlike traditional recommender systems, this project leverages NLP and transformer-based models to provide deep, meaningful suggestions.

---

## 🚀 Features

- 🔍 **Semantic Search**: Uses `all-MiniLM-L6-v2` from Hugging Face for context-aware recommendations.
- 💬 **Emotion Detection**: Analyzes tone using a transformer classifier to match book moods.
- 🧠 **Multi-Filter Logic**: Filter by category and emotional tone dynamically.
- ⚡ **Fast Vector DB**: Stores embeddings in `ChromaDB` for efficient nearest-neighbor search.
- 🖥️ **Gradio Interface**: Clean and interactive web-based UI to get suggestions instantly.
- 🔐 **Secure Config**: Stores API keys safely in `.env`.

---

## Demo

👉 [Check it out on Hugging Face] (https://huggingface.co/spaces/Arnav2211/Book-Recommender)

---

## 🛠️ Tech Stack

| Tool/Library             | Purpose                                       |
|--------------------------|-----------------------------------------------|
| `sentence-transformers`  | For semantic embeddings of book descriptions  |
| `transformers`           | Emotion classification using fine-tuned model |
| `langchain`              | Text loading and preprocessing                |
| `ChromaDB`               | Local vector similarity database              |
| `Gradio`                 | Web interface for user interaction            |
| `dotenv`                 | Manage secrets like HuggingFace token         |
| `Pandas & NumPy`         | Data preprocessing and manipulation           |

---

## 📦 Installation

```bash
git clone https://github.com/yourusername/book-recommender.git
cd book-recommender
python -m venv .venv
# Activate environment
# For Windows:
.venv\Scripts\activate
# For Mac/Linux:
source .venv/bin/activate
pip install -r requirements.txt
```

---

## 🔑 Environment Setup

Create a `.env` file in the root directory:

```env
HUGGINGFACEHUB_API_TOKEN=your_token_here
```

> Get your token from: https://huggingface.co/settings/tokens

---

## ▶️ Run the App

```bash
python gradio-dashboard.py
```

Visit the local Gradio URL provided to test the recommender.

---

## 📁 File Structure

```
book-recommender/
│
├── books_with_emotions.csv
├── tagged_description.txt
├── gradio-dashboard.py
├── sentiment-analysis.ipynb
├── text-classification.ipynb
├── .env
├── .gitignore
├── requirements.txt
└── README.md
```

---

## 💬 Example Query

```
"Looking for a humorous and uplifting novel about friendship"
```

System filters results semantically and emotionally to recommend appropriate titles.

---

## 📝 Resume Highlights

- Built a semantic book recommender using Hugging Face Sentence Transformers and ChromaDB.
- Integrated zero-shot emotion detection to fine-tune recommendations.
- Designed an interactive Gradio UI for real-time book suggestions.
- Leveraged LangChain and vector databases for scalable search architecture.

---

## 📄 License

This project is licensed under the MIT License. Feel free to use, adapt, and share it.