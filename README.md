# 🤖 AutoRAG: Autonomous RAG with GPT-4o and Vector Database

An advanced Autonomous Retrieval-Augmented Generation (RAG) system that combines document knowledge with real-time web search capabilities. Built with OpenAI's GPT-4o and PgVector database, this system provides intelligent, context-aware responses by seamlessly integrating uploaded documents with live web information.

## 🌟 Features

### Core Functionality
- **Autonomous RAG**: Intelligent retrieval and generation without manual intervention
- **Document Knowledge Base**: Upload and process PDF documents for knowledge extraction
- **Web Search Integration**: Real-time web search using DuckDuckGo
- **Persistent Storage**: PostgreSQL with PgVector for efficient vector storage
- **Chat Interface**: Interactive conversational interface
- **Context-Aware Responses**: Combines document and web knowledge intelligently

### Advanced Capabilities
- **Intelligent Retrieval**: Automatically selects relevant information sources
- **Multi-Source Synthesis**: Combines information from documents and web
- **Conversation Memory**: Maintains context across multiple interactions
- **Vector Similarity Search**: Efficient semantic search through documents
- **Real-time Updates**: Incorporates latest web information
- **Scalable Architecture**: Handles large document collections

## 🚀 Getting Started

### Prerequisites
- Python 3.8 or higher
- OpenAI API key
- Docker (for PgVector database)
- Sufficient storage for documents and vectors

### Installation

1. **Clone the repository**
   ```bash
   git clone https://github.com/rchhabra13/portfolio-projects.git
   cd portfolio-projects/autonomous_rag
   ```

2. **Install dependencies**
   ```bash
   pip install -r requirements.txt
   ```

3. **Set up PgVector database**
   ```bash
   docker run -d \
     -e POSTGRES_DB=ai \
     -e POSTGRES_USER=ai \
     -e POSTGRES_PASSWORD=ai \
     -e PGDATA=/var/lib/postgresql/data/pgdata \
     -v pgvolume:/var/lib/postgresql/data \
     -p 5532:5432 \
     --name pgvector \
     phidata/pgvector:16
   ```

4. **Set up API keys**
   ```bash
   export OPENAI_API_KEY="your-openai-api-key-here"
   ```

5. **Run the application**
   ```bash
   streamlit run autorag.py
   ```

6. **Access the application**
   - Open your browser to `http://localhost:8501`
   - Upload PDF documents to build your knowledge base
   - Start chatting with the AI assistant

## 💡 Usage Examples

### Document-Based Queries
```
"What are the main findings in the uploaded research paper?"
"Summarize the key points from the business report."
"What methodology was used in this study?"
```

### Web-Enhanced Queries
```
"Find the latest developments related to the topics in my documents."
"What are the current market trends for the technologies mentioned?"
"Are there any recent updates to the regulations discussed in the PDF?"
```

### Combined Knowledge Queries
```
"Compare the information in my documents with the latest industry news."
"What additional context can you provide about the concepts in my research?"
"How do the findings in my paper relate to current market conditions?"
```

## 🛠️ Technical Architecture

### Core Technologies
- **Framework**: Agno AI Agent Framework
- **Language Model**: OpenAI GPT-4o
- **Vector Database**: PostgreSQL with PgVector extension
- **Web Search**: DuckDuckGo integration
- **UI**: Streamlit for user interface
- **Document Processing**: PyPDF2 for PDF parsing

### RAG Pipeline
1. **Document Upload**: PDF documents are uploaded and processed
2. **Text Extraction**: Text is extracted from PDF pages
3. **Chunking**: Documents are split into manageable chunks
4. **Embedding Generation**: Text chunks are converted to vector embeddings
5. **Vector Storage**: Embeddings are stored in PgVector database
6. **Query Processing**: User queries are processed and analyzed
7. **Retrieval**: Relevant chunks are retrieved from both documents and web
8. **Synthesis**: Information is combined and synthesized
9. **Response Generation**: Comprehensive answers are generated

## 📊 Supported Document Types

### Academic Papers
- Research papers and studies
- Conference proceedings
- Journal articles
- Theses and dissertations

### Business Documents
- Reports and whitepapers
- Financial statements
- Legal documents
- Policy documents

### Technical Documentation
- User manuals
- API documentation
- Technical specifications
- Code documentation

## 🔧 Configuration

### Environment Variables
```bash
OPENAI_API_KEY=your-openai-api-key
```

### Database Configuration
- **Host**: localhost
- **Port**: 5532
- **Database**: ai
- **User**: ai
- **Password**: ai

### Customization Options
- **Chunk Size**: Adjust text chunk size for better retrieval
- **Chunk Overlap**: Set overlap between chunks
- **Top K Results**: Number of relevant chunks to retrieve
- **Web Search Depth**: Control web search comprehensiveness
- **Response Length**: Limit response detail level

## 📈 Performance Features

- **Efficient Vector Search**: Optimized similarity search using PgVector
- **Intelligent Caching**: Reduces redundant processing
- **Parallel Processing**: Concurrent document and web processing
- **Memory Management**: Efficient handling of large document collections
- **Error Recovery**: Robust error handling and fallback mechanisms

## 🔒 Security & Privacy

- **Data Encryption**: All data encrypted in transit and at rest
- **API Security**: Secure API key management
- **Database Security**: Secure database connections
- **Privacy Compliance**: Follows data privacy best practices

## 🤝 Contributing

We welcome contributions from developers and AI enthusiasts:

1. Fork the repository
2. Create a feature branch
3. Make your changes
4. Add tests if applicable
5. Submit a pull request

### Areas for Contribution
- Additional document format support
- Improved retrieval algorithms
- Better web search integration
- Enhanced UI/UX
- Performance optimizations

## 📝 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## 🆘 Support

For support and questions:
- Create an issue in the GitHub repository
- Check the documentation
- Review the FAQ section

## 🔮 Roadmap

- [ ] Support for more document formats
- [ ] Advanced web search capabilities
- [ ] Multi-language support
- [ ] Real-time document updates
- [ ] Collaborative features
- [ ] API endpoint for integration
- [ ] Mobile app support
- [ ] Advanced analytics

## 📊 Use Cases

### Research & Academia
- Literature review assistance
- Research paper analysis
- Academic document summarization
- Knowledge synthesis

### Business & Legal
- Document analysis and review
- Market research integration
- Legal document processing
- Business intelligence

### Education
- Interactive learning materials
- Document-based Q&A
- Research assistance
- Knowledge exploration

### Personal Use
- Document organization
- Information retrieval
- Content summarization
- Research assistance

## 🙏 Acknowledgments

- OpenAI for the GPT-4o language model
- Agno framework for agent orchestration
- Streamlit for the user interface
- PostgreSQL and PgVector for vector storage
- DuckDuckGo for web search capabilities

---

**Note**: This application is designed for educational and research purposes. Always ensure you have the right to process and analyze the documents you upload.

<!-- Updated: 2025-09-16 -->

<!-- Updated: 2025-09-16 -->

<!-- Updated: 2025-09-16 -->

<!-- Updated: 2025-09-16 -->

<!-- Updated: 2025-09-16 -->

<!-- Updated: 2025-09-16 -->

<!-- Updated: 2025-09-16 -->

<!-- Updated: 2025-09-16 -->

<!-- Updated: 2025-09-16 -->

<!-- Updated: 2025-09-16 -->

<!-- Updated: 2025-09-16 -->
