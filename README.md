
---

<h1 align="center">
🌐 MultiPage RAG - Agent Assistant <br>  🤖 Chatbot Demo
</h1>

<h3 align="center">
All-in-one AI assistant powered by LLMs, RAG pipelines, and agents for PDF Q&A, web search, and content summarisation.
</h3>

Sometimes, during my studies and research, I wish I had an assistant to help search through website archives, find information from a vast number of papers, and summarise content. 📚 I built this app to make the research and learning process simpler and smarter. While it's still a work in progress, you can check out the code.

- This demo version of the app allows interaction with LLMs using Python and Streamlit framework.  
- It supports multiple AI models, including Groq's Gemma, llama3 and OpenAI GPT-3 and GPT-4 (you can add even more), and combines RAG pipelines with agent-based search tools.  
- LangChain was used for orchestration, and embeddings were generated with a HuggingFace model. 
- It can process PDFs by splitting them into chunks, perform web searches with agent tools using Google search, Arxiv, and Wikipedia, and summarise YouTube videos or web content.  

💡Easily adaptable for integration with other APIs or models with minimal changes.


## **Features**

Let's break it down, page by page:
- 🧑‍🏫 **PDF Q&A Assistant:** Upload multiple PDF files and get the most relevant answers to your questions.
- 🌐 **Web Search Agent:** Retrieve information from Google, Arxiv, and Wikipedia.
- ▶️ **Content Summariser:** Summarise YouTube videos or website text in seconds.
- 💬 **Friendly Chat:**  Enjoy fun, creative, and engaging conversations with an AI assistant. 


<p align="center">
  <img src="https://github.com/Duygu-Jones/Rag-Agent-Chatbot/blob/main/static/multipage-chatbot.gif">
</p>

## **How Does It Work?**

🧑‍🏫 **PDF Q&A Assistant**
- Upload your PDF files, which are processed by splitting them into chunks for efficient search using a vector database. Relevant answers are fetched with cosine similarity and TF-IDF scoring. If no matching data is found in the PDFs, the system explicitly informs the user that the answer is not available in the provided files.

🌐 **Web Search Agent**
- Search with accuracy using tools like Arxiv and Wikipedia integrations.Queries are processed with zero-shot reasoning to retrieve relevant articles and provide concise, informative summaries.

▶️ **Content Summariser (Web or Youtube URL)**
- Quickly summarise YouTube videos or website content by simply pasting the URL. The system fetches video descriptions or webpage text, processes the content using advanced language models, and generates clear, concise summaries. Ideal for saving time and quickly understanding lengthy materials.

💬 **Friendly Chat**
- Chat naturally with an advanced language model. This page uses context-aware responses to ensure human-like conversations, perfect for casual Q&A, brainstorming, and fun, friendly interactions.


## 🛠️**Tech Stack**

- **Framework**: Streamlit  
- **AI Models**: Groq's Gemma, OpenAI GPT  
- **Tools**: LangChain for RAG pipelines and agents , HuggingFace for embedding. 
- **Vector Storage**: ChromaDB  
- **Document Processing**: PyPDFLoader  
- **Web Tools**: DuckDuckGo for Google Search, Arxiv, and Wikipedia APIs


## ♻️**Usage**

**Check Out the Demo Video on Youtube**: [🌐MultiPage RAG - Agent - Assistant 🤖 Chatbot Demo](https://www.youtube.com/watch?v=umJJhAhOcNU). 

- ✅ **Select an API & Model**: Enter API keys in the sidebar.  
- ✅ **Navigate Between Pages**: 🧑‍🏫 **PDF Q&A**, 🌐 **Web Search**,▶️ **Summarise**, 💬 **Friendly Chat**.
- 💫 **Enjoy the Experience**: Interact through the streamlit chatbot interface.  


## ⬇️ **Installation**

1. **Clone the Repository**  
   ```bash
   git clone https://github.com/Duygu-Jones/Rag-Agent-Chatbot
   cd Rag-Agent-Chatbot
   ```

2. **Install Dependencies**  
   ```bash
   pip install -r requirements.txt
   ```

3. **Add API Keys**  
   Create a `.env` file and add your API keys:  
   ```plaintext
   GROQ_API_KEY= "your_groq_api_key"
   OPENAI_API_KEY= "your_openai_api_key"
   ```

4. **Run the Application**  
   ```bash
   streamlit run ChatBot.py
   ```


## **Directory Structure**

```plaintext
MultiPage-AI-Chatbot/
│-- pages/
│   │-- Summarise_Web_YT.py    # Summarise YouTube & web content
│   │-- Web_Search_Agent.py    # Web search functionality
│   │-- PDF_QA_Assistant.py    # PDF Q&A assistant
│
│-- utils.py                   # Shared utility functions
│-- ChatBot.py                 # Main app entry point
│-- static/                    # CSS styles, images
│-- requirements.txt           # Project dependencies
│-- README.md                  # Project documentation
│-- .env                       # API key storage
```


## 🤝**Contributing**

Contributions are welcome!  
- Fork the repository  
- Create a new branch: `feature/your-feature`  
- Submit a pull request


---


## 🌱 About Me

I'm Duygu Jones, a Data Scientist with a curiosity for learning and development in the fields of Machine Learning and Generative AI.

If you'd like to learn more about me and my work:
- **LinkedIn**: [Linkedin/duygujones](https://www.linkedin.com/in/duygujones/)
- **Website**: [duygujones.com](https://duygujones.vercel.app/)
- **Kaggle**: [kaggle.com/duygujones](https://www.kaggle.com/duygujones)
- **GitHub**: [github.com/Duygu-Jones](https://github.com/Duygu-Jones)
- **Medium**: [medium.com/@duygujones](https://medium.com/@duygujones)

Feel free to connect! I’d love to hear from you! 😊



## ✨ Acknowledgements

Thank you to the open-source community for providing tools, ideas, and making resources accessible to everyone. Your contributions and support mean so much! 🙏<br>
I hope this repository is helpful and contributes back to the community, inspiring and assisting others as well.

Happy coding! 👩‍💻✨

---

##### 📜 License

This repository is licensed under the MIT License. See the [LICENSE](LICENSE) file for more details.

---
