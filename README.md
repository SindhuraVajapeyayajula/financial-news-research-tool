📰 Financial News Research Tool 📈

It is a simple AI-powered news research tool that allows users to extract insights from multiple news articles. By providing URLs, the tool processes the content and answers user queries with relevant sources.

🚀 Features
🔗 Input multiple news article URLs
📄 Automatically loads and processes article content
✂️ Splits text into smaller chunks for better understanding
🧠 Uses OpenAI embeddings + FAISS for semantic search
❓ Ask questions based on the articles
📚 Returns answers along with source references

🏗️ Tech Stack
Frontend/UI: Streamlit
LLM: OpenAI (via LangChain)
Vector Store: FAISS
Embeddings: OpenAI Embeddings
Data Processing: LangChain Text Splitter + URL Loader
Environment Management: python-dotenv

📂 Project Structure
financial-news-research-tool-project/
│── main.py                     # Main Streamlit app
│── requirements.txt            # Dependencies
│── .env                        # API keys 
│── faiss_store_openai.pkl      # Saved vector database
│── notebooks/                  # Experiments & tutorials

💡 How It Works
User enters up to 3 news article URLs
Tool loads data using UnstructuredURLLoader
Text is split into chunks using RecursiveCharacterTextSplitter
Embeddings are created using OpenAI
Data is stored in FAISS vector database
User asks a question
Retrieval QA chain finds relevant chunks and generates answer

🖥️ Usage
Enter article URLs in the sidebar
Click "Process URLs"
Ask your question in the input box
Get:
✅ Answer
📚 Source references

📊 Example Use Cases
News summarization
Market research
Quick insights from multiple articles
Financial/news analysis

⚠️ Limitations
Works best with clean, text-based articles
Limited to URLs provided by user
Dependent on OpenAI API usage

🔮 Future Improvements
Support for PDFs and documents
More URLs input support
Better UI/UX
Caching and faster retrieval
Multi-language support

👨‍💻 Author
Developed as part of an AI/LLM-based project to demonstrate:
Retrieval-Augmented Generation (RAG)
Vector search using FAISS
Real-world NLP applications
