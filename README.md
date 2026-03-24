# LangGraph BMI Workflow

A simple, modular workflow built with **LangGraph** to calculate Body Mass Index (BMI) and categorize the result.

## 🚀 Overview

This project demonstrates the core concepts of LangGraph:
- **State Management**: Using `TypedDict` to pass data between nodes.
- **Nodes**: Independent functions for calculating (BMI = weight/height²) and categorizing (Normal, Overweight, etc.).
- **Graph Construction**: Building a linear flow from `START` to `END`.

## 🛠️ Prerequisites

- Python 3.11+
- [LangGraph](https://github.com/langchain-ai/langgraph)
- [LangChain](https://github.com/langchain-ai/langchain)

## 📦 Installation

To run the notebook, install the required packages:

```bash
pip install langgraph langchain
```

## 📖 Usage

1. Open `first_workflow.ipynb`.
2. Ensure you are using a Python environment with the prerequisites installed.
3. Run all cells to see the workflow in action.

## 📊 Workflow Logic

1. **Calculate Node**: Computes the BMI based on input `weight_kg` and `height_m`.
2. **Categorize Node**: Maps the BMI value to standard health categories:
   - **Underweight**: < 18.5
   - **Normal**: 18.5 - 24.9
   - **Overweight**: 25 - 29.9
   - **Obese**: ≥ 30
