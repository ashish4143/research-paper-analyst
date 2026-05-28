# Research Paper Analyst 🔬

An AI-powered research agent that uses the **Plan-and-Execute** architecture to analyze any research topic directly inside a Jupyter Notebook.

## Features
- **Web Search**: Uses Tavily to fetch up-to-date research papers and articles.
- **Dynamic Planning**: Leverages an LLM to formulate a targeted 3-5 step research plan based on your objective.
- **Autonomous Execution**: Executes each step of the plan against the retrieved content to extract insights.
- **Report Generation**: Synthesizes all findings into a structured, well-formatted Markdown report with source citations.
- **Self-Contained**: Everything runs entirely within a single, humanized Jupyter Notebook (`research_analyst.ipynb`).

## Technologies Used
- LangGraph
- LangChain
- Tavily Search API
- OpenAI GPT-4o-mini
- Python (Jupyter Notebook)

## Setup Instructions

1. Clone the repository:
   ```bash
   git clone https://github.com/ashish4143/research-paper-analyst.git
   cd research-paper-analyst
   ```
2. Open `research_analyst.ipynb` in VS Code or Jupyter.
3. Create a `.env` file in the root directory and add your API keys:
   ```env
   OPENAI_API_KEY=your_openai_api_key
   TAVILY_API_KEY=your_tavily_api_key
   ```
   *(If you don't create this file, the notebook will safely prompt you to enter the keys when you run it).*
4. Run all cells in the notebook!

## Usage
Simply call the `analyze()` function with your research question at the bottom of the notebook:
```python
report = analyze("latest trends in EV batteries")
```
