# YT_Q-A_RAG 🎥📚

A **RAG-based YouTube Video Q&A Platform** that allows users to ask questions from YouTube videos, generate **AI-powered notes**, **flashcards**, and **quizzes**, with **multilingual video support** and **downloadable study materials**.

This project is designed for **students, educators, and self-learners** who want to convert long YouTube videos into structured, searchable, and interactive knowledge.

---

## 🚀 Features

### 🔍 YouTube Video Q&A (RAG-based)

* Ask natural language questions from YouTube videos
* Uses **Retrieval-Augmented Generation (RAG)** for accurate answers
* Context-aware responses based on video transcripts

### 📝 Smart Notes Generation

* Auto-generated **structured notes** from videos
* Bullet points, headings, and summaries
* Download notes as **PDF / TXT / Markdown**

### 🧠 Flashcard Generator

* Automatically generates **Q–A flashcards**
* Useful for quick revision and spaced repetition
* Exportable for later use

### ❓ Quiz Generator

* MCQs and short-answer questions from video content
* Difficulty-based quiz generation
* Instant evaluation and feedback

### 🌍 Multilingual Support

* Supports videos in **multiple languages**
* Auto language detection
* Translation + multilingual Q&A support

### ⬇️ Downloads

* Notes
* Flashcards
* Quiz questions

---

## 🏗️ System Architecture

```
YouTube URL
   ↓
Transcript Extraction
   ↓
Text Chunking
   ↓
Embedding Generation
   ↓
Vector Database (FAISS / Chroma)
   ↓
Retriever + LLM (RAG)
   ↓
Q&A | Notes | Flashcards | Quiz
```

---

## 🛠️ Tech Stack

### Backend

* **Python**
* **FastAPI / Flask**
* **LangChain**
* **FAISS / ChromaDB**
* **Hugging Face Transformers**
* **YouTube Transcript API**

### LLMs

* Hugging Face Models (e.g. `flan-t5`, `mistral`, `llama`)
* Open-source embedding models

### Frontend

* **Streamlit / React.js**
* Tailwind CSS (optional)

### Other Tools

* Sentence Transformers
* Google Translate / MarianMT
* PDF generation tools

---

## 📂 Project Structure

```
YT_Q-A_RAG/
│
├── backend/
│   ├── app.py
│   ├── rag_pipeline/
│   │   ├── loader.py
│   │   ├── chunker.py
│   │   ├── embeddings.py
│   │   ├── retriever.py
│   │   └── qa_engine.py
│   ├── notes_generator.py
│   ├── flashcard_generator.py
│   ├── quiz_generator.py
│   ├── translator.py
│   └── requirements.txt
│
├── frontend/
│   ├── streamlit_app.py
│   └── components/
│
├── data/
│   ├── transcripts/
│   ├── embeddings/
│   └── outputs/
│
├── README.md
└── .env
```

---

## ⚙️ Installation & Setup

### 1️⃣ Clone the Repository

```bash
git clone https://github.com/your-username/YT_Q-A_RAG.git
cd YT_Q-A_RAG
```

### 2️⃣ Create Virtual Environment

```bash
python -m venv venv
source venv/bin/activate  # Linux/Mac
venv\Scripts\activate     # Windows
```

### 3️⃣ Install Dependencies

```bash
pip install -r backend/requirements.txt
```

### 4️⃣ Environment Variables

Create a `.env` file:

```
HUGGINGFACE_API_KEY=your_key_here
OPENAI_API_KEY=optional
```

### 5️⃣ Run Backend

```bash
python backend/app.py
```

### 6️⃣ Run Frontend

```bash
streamlit run frontend/streamlit_app.py
```

---

## 📌 Usage

1. Paste a **YouTube video URL**
2. Select language (or auto-detect)
3. Ask questions from the video
4. Generate:

   * Notes
   * Flashcards
   * Quiz
5. Download learning materials

---

## 📊 Example Use Cases

* Exam preparation from lectures
* Converting podcasts into notes
* Multilingual learning
* Interview prep from YouTube tutorials
* Revision using flashcards & quizzes

---

## 🔐 Security & Privacy

* No video content is stored permanently
* Only transcripts and embeddings are cached locally
* API keys are secured via environment variables

---

## 🧪 Future Enhancements

* User authentication
* Progress tracking dashboard
* Voice-based Q&A
* Mobile-friendly UI
* Knowledge graph visualization

---

## 🤝 Contributing

Contributions are welcome!

1. Fork the repository
2. Create a new branch
3. Commit your changes
4. Open a Pull Request

---

## 📜 License

This project is licensed under the **MIT License**.

---

## 🙌 Acknowledgements

* Hugging Face
* LangChain
* YouTube Transcript API
* Open-source community

---

## 📬 Contact

**Author:** Prankit Bajpai
**Project:** YT_Q-A_RAG

If you like this project ⭐ star the repository!

