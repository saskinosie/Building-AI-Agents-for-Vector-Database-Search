# Building AI Agents for Vector Database Search

![Python](https://img.shields.io/badge/python-3.8+-blue.svg)
![License](https://img.shields.io/badge/license-MIT-green.svg)
![Weaviate](https://img.shields.io/badge/weaviate-4.x-orange.svg)

> **Learn to build intelligent AI agents that transform complex vector database queries into simple, natural language interactions.**

## Overview

Vector databases are powerful, but querying them effectively requires expertise. What if you could use natural language instead of writing complex queries? This hands-on workshop teaches you to build AI agents that:

✅ **Optimize queries automatically** - Transform vague user questions into precise vector searches
✅ **Generate filters dynamically** - Create database filters on-the-fly based on context
✅ **Combine multiple techniques** - Layer query optimization with smart filtering for best results
✅ **Simplify complexity** - Make vector search accessible to non-technical users

**The key insight**: AI agents aren't magic—they're well-structured prompts + intelligent parsing + API orchestration. And you can build them yourself.

## What You'll Learn

This progressive tutorial takes you from vector database basics to building production-ready agents:

### 📘 [Lesson 1: Vector Database Queries](1-vector-database-queries.ipynb)
**Foundation**: Understanding vector search and its challenges
- Set up a Weaviate vector database with financial contracts
- Perform semantic searches with vector embeddings
- Apply filters for precise results
- Use generative search for question answering
- **Key insight**: Manual query optimization is time-consuming and requires expertise

### 🤖 [Lesson 2: Building Agents](2-building-agents.ipynb)
**Core skills**: Creating agents that automate query optimization and filtering
- Build simple conversational agents with memory
- Create query optimization agents
- Develop dynamic filter generation agents
- **Combine both techniques** for powerful, automated search
- **Key insight**: Agents make vector search accessible and efficient

## Why This Matters

**Traditional approach**: Users need to understand vector embeddings, similarity scores, filter syntax, and database schemas.

**With agents**: Users ask questions in natural language. The agent handles the complexity.

**Real-world impact**:
- Customer support teams can search documentation without training
- Legal professionals can find contracts without learning query syntax
- Product teams can prototype search features in minutes, not weeks

## Quick Start

### Prerequisites
- Python 3.8+ (for local setup)
- Basic understanding of APIs and async programming
- OpenAI API key ([get one here](https://platform.openai.com/api-keys))
- Weaviate Cloud account ([free tier available](https://console.weaviate.cloud/))

### Option 1: Run in Google Colab (Recommended - No Installation Required)
Click the "Open in Colab" badges in each notebook to run directly in your browser. Perfect for getting started quickly!

### Option 2: Run Locally

**Setup:**
```bash
# Clone the repository
git clone https://github.com/YOUR_USERNAME/dsd-building-ai-agents-with-vector-db.git
cd dsd-building-ai-agents-with-vector-db

# Create virtual environment
python -m venv .venv
source .venv/bin/activate  # On Windows: .venv\Scripts\activate

# Install dependencies (includes Jupyter)
pip install -r requirements.txt

# Configure credentials
cp .env.example .env
# Edit .env with your API keys (see setup instructions below)
```

**Run the notebooks:**
```bash
# Option A: Jupyter Notebook
jupyter notebook

# Option B: Jupyter Lab
jupyter lab

# Option C: VS Code
# Open the folder in VS Code and use the built-in notebook viewer
```

## Create a Weaviate Cloud instance

  * Head to [Weaviate Cloud console](https://console.weaviate.cloud/) and log in, or create a new account.
  * Create a free `Sandbox` cluster. Give it a name, select the cloud region and press "Create".
  * Copy your REST endpointe and paste it into your .env as WEAVIATE_URL
  * Create an API key with admin privileges and copy and paste it into your .env as WEAVIATE _KEY

![wcd create cluster - step 1](img/wcd-create-cluster-1.jpg)
![wcd create cluster - step 2](img/wcd-create-cluster-2.jpg)
![wcd create cluster - step 3](img/wcd-create-rest-endpoint.png)
![wcd create cluster - step 4](img/wcd-create-apikey-1.png)
![wcd create cluster - step 5](img/wcd-create-apikey2.png)




## Environment Configuration

After creating your Weaviate cluster, configure your environment variables:

1. **Copy the example file**
```bash
cp .env.example .env
```

2. **Add your credentials to `.env`**

Find your Weaviate credentials in the [WCD console](https://console.weaviate.cloud/):
- `WEAVIATE_URL` = Your cluster's `REST Endpoint`
- `WEAVIATE_KEY` = `Admin` key from the `API Keys` section
- `OPENAI_API_KEY` = Your OpenAI API key from [platform.openai.com](https://platform.openai.com/api-keys)

## Project Structure

```
├── 1-vector-database-queries.ipynb    # Introduction to vector search
├── 2-building-agents.ipynb             # Building AI agents (hands-on)
├── complete/                            # Completed notebooks with solutions
│   └── 2-building-agents-complete.ipynb
├── img/                                 # Setup screenshots
├── requirements.txt                     # Python dependencies
├── .env.example                         # Template for environment variables
└── README.md                            # You are here!
```

## Key Technologies

- **[Weaviate](https://weaviate.io/)** - Open-source vector database
- **[Pydantic AI](https://ai.pydantic.dev/)** - Framework for building production-grade AI agents
- **[OpenAI GPT-4o-mini](https://platform.openai.com/)** - Language model for query optimization
- **[HuggingFace Datasets](https://huggingface.co/datasets/weaviate/agents)** - Pre-vectorized contract data

## Use Cases

This tutorial prepares you to build:

- 🔍 **Semantic search systems** - Find documents by meaning, not just keywords
- 📚 **Knowledge base assistants** - Query company documentation in natural language
- ⚖️ **Legal document retrieval** - Search contracts and policies intelligently
- 🛒 **E-commerce search** - Product discovery with natural language
- 💼 **HR systems** - Find relevant policies and employee records
- 🏥 **Medical record search** - HIPAA-compliant clinical data retrieval

## Contributing

Found a bug? Have an improvement? Contributions are welcome!

1. Fork the repository
2. Create a feature branch (`git checkout -b feature/amazing-addition`)
3. Commit your changes (`git commit -m 'Add amazing feature'`)
4. Push to the branch (`git push origin feature/amazing-addition`)
5. Open a Pull Request

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## Acknowledgments

- Built with [Weaviate](https://weaviate.io/) vector database
- Dataset hosted on [HuggingFace](https://huggingface.co/datasets/weaviate/agents)

## Resources & Further Reading

- 📖 [Weaviate Documentation](https://weaviate.io/developers/weaviate)
- 🤖 [Pydantic AI Documentation](https://ai.pydantic.dev/)
- 🧠 [Understanding Vector Embeddings](https://weaviate.io/blog/vector-embeddings-explained)
- 🔧 [Query Agent Deep Dive](https://docs.weaviate.io/agents/query)

---

**Questions or feedback?** Open an issue or reach out on [LinkedIn](https://www.linkedin.com/in/YOUR_PROFILE)!

