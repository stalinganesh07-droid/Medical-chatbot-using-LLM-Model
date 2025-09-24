# Medical-chatbot-using-LLM-Model

🩺 Medical Chatbot using LLM (RAG-powered)

An AI-powered Medical Chatbot that leverages LangChain, OpenAI LLMs, and Pinecone for retrieval-augmented generation (RAG).
It provides context-aware medical responses by combining LLM reasoning with a vector database of medical knowledge.

⚠️ Disclaimer: This chatbot is for educational and informational purposes only. It is not a substitute for professional medical advice.

🚀 Features

🧠 LLM + RAG → Combines OpenAI models with Pinecone vector search.

📚 Medical Knowledge Base → Ingests PDFs & text docs (via pypdf + sentence-transformers).

💬 Conversational Chatbot → Answers medical queries naturally.

🌐 Flask API Support → Can be deployed as a web app.

🧾 Notebook Workflow → Easy to experiment with RAG pipelines in Jupyter/Colab.

🛠️ Tech Stack

LLM Backend: OpenAI (via langchain-openai)

RAG Framework: LangChain (0.3.26)

Vector DB: Pinecone (langchain-pinecone)

Embeddings: sentence-transformers

PDF Processing: pypdf

Web API: Flask (3.1.1)

Environment: Jupyter Notebook + Python 3.10+

📂 Project Structure
Medical-Chatbot-using-LLM-Model/
│── notebooks/
│   └── rag_medical_chatbot.ipynb   # Main Jupyter Notebook
│── src/
│   ├── data_loader.py              # Load + preprocess PDFs
│   ├── vector_store.py             # Pinecone integration
│   ├── chatbot.py                  # LangChain pipeline
│   └── app.py                      # Flask app (optional)
│── requirements.txt
│── .env                            # API keys
│── README.md

⚙️ Installation

Clone repo

git clone https://github.com/your-username/Medical-Chatbot-using-LLM-Model.git
cd Medical-Chatbot-using-LLM-Model


Create venv

python -m venv venv
source venv/bin/activate   # macOS/Linux
venv\Scripts\activate      # Windows


Install dependencies

pip install -r requirements.txt


Setup environment variables
Create a .env file in the project root:

PINECONE_API_KEY=your_pinecone_api_key
OPENAI_API_KEY=your_openai_api_key

▶️ Usage
🧾 Run inside Notebook

Open Jupyter Notebook:

jupyter notebook notebooks/rag_medical_chatbot.ipynb

🌐 Run Flask API (Optional)
python src/app.py


Then open: http://127.0.0.1:5000

📦 requirements.txt
langchain==0.3.26
flask==3.1.1
sentence-transformers==5.1.0
pypdf==5.6.1
python-dotenv==1.1.0
langchain-pinecone==0.2.8
langchain-openai==0.3.24
langchain-community==0.3.26
-e .

🔮 Future Scope

🔊 Speech integration (patient ↔ doctor voice interface)

📊 Medical report summarization

🌎 Multi-language medical chatbot

🏥 EHR (Electronic Health Record) integration

📜 License

MIT License – Free for academic & personal use.
