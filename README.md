# LangGraph Workflows

This repository contains intelligent and modular workflows built with **LangGraph** to demonstrate core concepts like state management, linear routing, and parallel execution.

## 🚀 Included Workflows

### 1. BMI Calculator (`first_workflow.ipynb`)

A linear workflow to calculate Body Mass Index (BMI) and categorize the result.

- **Calculate Node**: Computes BMI (weight/height²).
- **Categorize Node**: Maps BMI to standard health categories (Underweight, Normal, Overweight, Obese).

### 2. Parallel Cricket Statistics (`second_workfolw.ipynb`)

A parallel execution workflow that computes multiple statistics simultaneously for a cricket player's match performance.

- **Parallel Nodes**:
  - `strike_rate`: Computes `(runs / balls) * 100`
  - `dot_ball_percent`: Computes `(dot_balls / balls) * 100`
  - `boundary_percent`: Computes `(boundaries / balls) * 100`
  - `summary`: Generates a natural language summary of the performance.
- **Graph Construction**: Fans-out from `START` to all four metric nodes simultaneously, then fans-in to `END`.

## 🛠️ Prerequisites

- Python 3.11+
- [LangGraph](https://github.com/langchain-ai/langgraph)
- [LangChain](https://github.com/langchain-ai/langchain)
- `langchain-openai` (optional, for LLM steps)

## 📦 Installation

To run the notebooks, install the required packages:

```bash
pip install langgraph langchain langchain-openai
```

## 📖 Usage

1. Open `first_workflow.ipynb` or `second_workfolw.ipynb`.
2. Ensure you are using a Python environment with the prerequisites installed.
3. Run all cells to see the workflows in action.
