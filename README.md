# 📚 Conversational RAG with PDF Uploads & Chat History

Ever wish you could just *talk* to your PDFs? This project is a fun little app I built that lets you upload PDF files and have a natural conversation with their content. It remembers your questions, understands context, and gives snappy, accurate answers — all through a clean Streamlit interface.

Built using **LangChain**, **Groq’s Gemma 2 model**, and **HuggingFace embeddings**, this app showcases how Retrieval-Augmented Generation (RAG) can be used to turn static documents into dynamic conversations.

> 📁 GitHub Repo: [https://github.com/Saketh35/Conversational-RAG-with-PDF-Uploads-Chat-History](https://github.com/Saketh35/Conversational-RAG-with-PDF-Uploads-Chat-History)

---

## ✨ Features

* 🧠 Conversational Q\&A over multiple PDF files
* 💬 Maintains **chat history** across sessions using a session ID
* 📄 Supports **multiple PDF uploads**
* 🔍 Uses document splitting & semantic search to retrieve relevant info
* 🧰 Powered by **Groq’s blazing-fast LLMs** and **HuggingFace embeddings**
* 🖥️ Clean, simple interface using **Streamlit**

---

## 🛠️ Tech Stack

* `Streamlit` – for the interactive UI
* `LangChain` – to wire together RAG components
* `Groq` + `Gemma 2` – for fast and efficient language model inference
* `HuggingFace` – for embedding PDFs
* `Chroma` – for vector storage & retrieval
* `Python-dotenv` – to manage API keys securely
* `PyPDF` – for loading PDF documents

---

## 🚀 Getting Started

### 1. Clone the repo

```bash
git clone https://github.com/Saketh35/Conversational-RAG-with-PDF-Uploads-Chat-History.git
cd Conversational-RAG-with-PDF-Uploads-Chat-History
```

### 2. Set up your environment

It's recommended to use a virtual environment:

```bash
python -m venv venv
source venv/bin/activate  # or venv\Scripts\activate on Windows
```

### 3. Install dependencies

```bash
pip install -r requirements.txt
```

### 4. Set up your `.env` file

Create a `.env` file in the root directory with the following:

```env
HF_TOKEN=your_huggingface_token_here
```

You’ll also enter your **Groq API key** inside the app when prompted.

---

## 🧪 How to Use

1. Run the app:

```bash
streamlit run app.py
```

2. In the browser:

   * Enter your **Groq API key**
   * Choose a **Session ID** (can be anything, like your name)
   * Upload one or more **PDF files**
   * Ask any question based on their content!
   * The app will remember the conversation as long as the session ID stays the same.

---

## ⚠️ Notes & Known Issues

* ❗ If you upload a large PDF, it might take a moment to process and chunk the content.
* 🧠 Chat memory is managed in memory per session — it's not persistent yet.
* 🔐 API keys are handled securely, but make sure not to commit your `.env` file.
* 🧪 This is an experimental app — not production-ready but great for learning or demos.

---

## 🤝 Let’s Collaborate!

I'm always looking to improve this or hear how others might use it. If you have feedback, suggestions, or want to contribute, feel free to [open an issue](https://github.com/Saketh35/Conversational-RAG-with-PDF-Uploads-Chat-History/issues) or a pull request!

You can also ⭐ the repo if you found it helpful — it really means a lot :)

---

Thanks for checking it out!
Happy chatting with your PDFs! 💬📄
