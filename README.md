# LangGraph Learning & Projects

A comprehensive repository for learning and implementing LangGraph workflows using LangChain, demonstrating various use cases from simple workflows to complex chatbot applications.

## 📁 Project Structure

### 📓 Tutorial Notebooks

Jupyter notebooks demonstrating different LangGraph concepts and workflows:

- **0_test_installation.ipynb** - Installation verification and setup guide
- **1_bmi_workflow.ipynb** - BMI calculator workflow
- **2_simple_workflow.ipynb** - Basic workflow introduction
- **3_prompt_chaining.ipynb** - Chaining multiple prompts together
- **4_batman_workflow.ipynb** - Batman-themed workflow example
- **5_UPSC_essay_workflow.ipynb** - Essay writing workflow for UPSC preparation
- **6_quadratic_equation.ipynb** - Mathematical problem-solving workflow
- **7_review_reply_workflow.ipynb** - Review and reply generation workflow
- **8_X_post_generator.ipynb** - Social media post generation using LangGraph
- **9_basic_chatbot.ipynb** - Basic chatbot implementation

### 🤖 Chatbot Application

**`chatbot_using_langgraph/`** - Full-stack chatbot application with streaming support

- **langgraph_backend.py** - LangGraph backend logic for the chatbot
- **streamlit_frontend.py** - Basic Streamlit frontend
- **streamlit_frontend_threading.py** - Frontend with threading support
- **streamlit_frontennd_streaming.py** - Frontend with streaming capabilities
- **requirements.txt** - Python dependencies

### 📚 Additional Folders

- **Challenges_in_langchain/** - Challenge problems and solutions
- **Sequential_Workflow/** - Sequential workflow examples and patterns

## 🚀 Getting Started

### Prerequisites

- Python 3.8+
- conda or pip for package management
- OpenAI API key (for LLM capabilities)

### Installation

1. Clone the repository:
```bash
git clone <repository-url>
cd Langraph
```

2. Create and activate conda environment:
```bash
conda env create -n langgraph python=3.10
conda activate langgraph
```

3. Install dependencies:
```bash
pip install -r chatbot_using_langgraph/requirements.txt
```

4. Set up environment variables:
```bash
# Create a .env file with your API keys
echo "OPENAI_API_KEY=your_api_key_here" > .env
```

## 📦 Key Dependencies

- **langchain** (0.3.27) - LLM framework and tools
- **langgraph** (0.6.1) - Graph-based workflow orchestration
- **langchain-openai** (0.3.28) - OpenAI integration
- **streamlit** - Web UI framework
- **pandas** & **numpy** - Data processing
- **pydantic** - Data validation

## 🎯 Usage

### Run Tutorial Notebooks

```bash
jupyter notebook 1_bmi_workflow.ipynb
```

### Run Chatbot Application

```bash
cd chatbot_using_langgraph
streamlit run streamlit_frontend_threading.py
```

For different versions:
- **Basic**: `streamlit run streamlit_frontend.py`
- **With Threading**: `streamlit run streamlit_frontend_threading.py`
- **With Streaming**: `streamlit run streamlit_frontennd_streaming.py`

## 💡 Key Concepts Covered

- **Workflow Orchestration** - Building complex workflows using LangGraph
- **Prompt Chaining** - Sequencing multiple LLM calls
- **Message Passing** - Thread-based conversation management
- **Streaming Responses** - Real-time response generation
- **Stateful Conversations** - Maintaining conversation history and context

## 🔧 Architecture

### Backend (LangGraph)
- Defines the conversation graph and message flow
- Manages state and thread configuration
- Handles LLM interactions via LangChain

### Frontend (Streamlit)
- Interactive chat interface
- Session state management
- Thread ID tracking for multi-turn conversations
- Support for streaming and threaded execution

## 📝 Notes

- The chatbot uses thread IDs to manage separate conversation sessions
- Supports both streaming and non-streaming message delivery
- Compatible with various OpenAI models (configurable)

## 🤝 Contributing

Feel free to add more workflow examples and improvements!

## 📄 License

This repository is for educational purposes.

---

**Last Updated**: February 2026
