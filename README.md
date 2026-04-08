# Learning LangGraph

This repository contains a collection of Jupyter Notebooks dedicated to learning and implementing various concepts and patterns using [LangGraph](https://python.langchain.com/docs/langgraph/). The notebooks are structured progressively to build up knowledge from basic concepts to advanced agent workflows.

## Project Structure

The core learning materials are located within the `Notebooks/` directory. Each notebook focuses on a specific feature, component, or design pattern:

- **`1_basics.ipynb`**: Introduction to foundational LangGraph components (State, Nodes, Edges).
- **`2_Pydantic.ipynb`**: Structuring LLM outputs and ensuring structured data via Pydantic.
- **`3_prompts.ipynb`**: Crafting and managing prompts inside graph states.
- **`4_tools.ipynb`**: Defining and binding external tools for your agents to use.
- **`5_ReAct_agents.ipynb`**: Building Reason + Act (ReAct) agents that can iteratively solve problems using tools.
- **`6_Parallelization.ipynb`**: Executing multiple graph nodes concurrently to optimize performance.
- **`7_Routing.ipynb`**: Implementing conditional logic (conditional edges) to route tasks through specialized branches.
- **`8_Orchestrator&Worker.ipynb`**: Exploring the orchestrator-worker pattern, where a manager node delegates independent tasks to specialized sub-agents.
- **`9_Generator_Evaluator.ipynb`**: The generator-evaluator design pattern for iterative improvement, critiquing, and refinement of LLM outputs.
- **`10_Memory.ipynb`**: Implementing memory (checkpointers) to maintain persistent state across multiple interactions.

## Setup & Dependencies

This project relies on `uv` for fast dependency management, as defined in the `pyproject.toml` and `uv.lock` files.

**Prerequisites:**
- Python `>= 3.10`
- `uv` installed (`pip install uv`)

### Installation Steps:

1. **Clone the repository and sync dependencies:**
   ```bash
   uv sync
   ```

2. **Activate the local environment:**
   ```bash
   # On Windows
   .venv\Scripts\activate
   
   # On macOS/Linux
   source .venv/bin/activate
   ```

3. **Environment Variables:**
   A `.env` file is required in the root directory to store your API keys (e.g., `OPENAI_API_KEY` or `GROQ_API_KEY`). Ensure this file is populated before running the notebooks.

## Quick Start

To interact with the codebase, simply start your Jupyter environment from the root directory:

```bash
jupyter notebook
```
Navigate to the `Notebooks/` folder and work through them sequentially.
