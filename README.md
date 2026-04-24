# 🤖 Agent Evals Tutorial

A comprehensive Google Colab-ready tutorial for learning agent evaluation with LangSmith, LangChain, and LangGraph.

---

## 🚀 Quick Start - Start Here!

**Start with the executable tutorial:**
```bash
# Just open in Colab: 01_executable_tutorial.ipynb
# Or run locally:
pip install -r requirements.txt
jupyter notebook 01_executable_tutorial.ipynb
```

**Then create your presentation:**
1. Copy `GEMMA_SLIDE_PROMPT.txt`
2. Paste into Google Gemini/Gemma
3. Ask to create slides

This tutorial teaches you everything about building and evaluating AI agents, from basics to advanced evaluation techniques.

### What You'll Learn

| Module | Content | Notebooks |
|--------|---------|----------|
| **PART 1** | LLM Fundamentals | 3 |
| **PART 2** | Agents Basics | 5 |
| **PART 3** | Agent Frameworks | 4 |
| **PART 4** | Observability | 3 |
| **PART 5** | Agent Evals | 7 |

**Total: 22 Notebooks** 😎

---

## 🚀 Quick Start

### 1. Open in Google Colab

Click any notebook to open in Colab, or run locally:

```bash
# Clone the repo
git clone https://github.com/your-repo/AgentEvals.git
cd AgentEvals

# Install requirements
pip install -r requirements.txt

# Run a notebook
jupyter notebook
```

### 2. Set Up API Keys

You'll need:
- **OpenAI API Key**: Get at https://platform.openai.com/api-keys
- **LangSmith API Key**: Get at https://smith.langchain.com (optional, for tracing)

Set in your environment:
```bash
export OPENAI_API_KEY="sk-..."
export LANGCHAIN_API_KEY="ls-..."
```

---

## 📖 Notebooks by Section

### PART 1: LLM Fundamentals

| Notebook | Description |
|----------|-------------|
| 01_introduction_to_llms | What LLMs are, API calls |
| 02_prompts_and_tokens | Tokenization, few-shot, CoT |
| 03_llm_limitations_and_errors | Hallucinations, context, errors |

### PART 2: Agents Basics

| Notebook | Description |
|----------|-------------|
| 01_what_are_agents | Agent loop, components |
| 02_tools_and_function_calling | Tool creation, schema |
| 03_routers_and_skills | Routing, multi-skill |
| 04_memory_and_state | Memory, state, persistence |
| 05_analogy_junior_developer | Mental model analogy |

### PART 3: Agent Frameworks

| Notebook | Description |
|----------|-------------|
| 01_langchain_agents | LangChain + LCEL |
| 02_langgraph_agents | State graphs, nodes |
| 03_combined_example | Research agent |
| 04_debugging_agents | Common bugs |

### PART 4: Observability

| Notebook | Description |
|----------|-------------|
| 01_traditional_vs_agent | Traditional vs agent observability |
| 02_introduction_to_langsmith | LangSmith overview |
| 03_tracing_basic_agents | Adding tracing |

### PART 5: Agent Evals ⭐

| Notebook | Description |
|----------|-------------|
| 01_what_are_agent_evals | What evals are |
| 02_types_of_evals | Output, trajectory, RAG, safety |
| 03_creating_eval_datasets | Building test datasets |
| 04_building_evaluators | LLM-as-Judge, assertions |
| 05_running_evals_and_langsmith | Running evaluations |
| 06_error_propagation_examples | Common errors |
| 07_final_project_end_to_end | Complete project! |

---

## 🎯 Key Concepts

### What Are Agents?
- **LLM + Loop + Tools + Memory**
- Autonomous, goal-directed systems

### What Are Agent Evals?
- **Output Evaluation** - Is the answer correct?
- **Trajectory Evaluation** - Did it use the right tools?
- **RAG Evaluation** - Is it grounded in facts?
- **Safety Evaluation** - No hallucinations?

### Why Traditional Tests Don't Work
- **Probabilistic** - Same input can give different outputs
- **Fuzzy** - Multiple valid answers
- **Multi-step** - Path matters, not just output

---

## 📊 Project Structure

```
AgentEvals/
├── PART_1_LLM_Fundamentals/
│   ├── 01_introduction_to_llms.ipynb
│   ├── 02_prompts_and_tokens.ipynb
│   └── 03_llm_limitations_and_errors.ipynb
├── PART_2_Agents_Basics/
│   ├── 01_what_are_agents.ipynb
│   ├─�� 02_tools_and_function_calling.ipynb
│   ├── 03_routers_and_skills.ipynb
│   ├── 04_memory_and_state.ipynb
│   └── 05_analogy_junior_developer.ipynb
├── PART_3_Agent_Frameworks/
│   ├── 01_langchain_agents.ipynb
│   ├── 02_langgraph_agents.ipynb
│   ├── 03_combined_example.ipynb
│   └── 04_debugging_agents.ipynb
├── PART_4_Observability/
│   ├── 01_traditional_vs_agent_observability.ipynb
│   ├── 02_introduction_to_langsmith.ipynb
│   └── 03_tracing_basic_agents.ipynb
├── PART_5_Agent_Evals/
│   ├── 01_what_are_agent_evals.ipynb
│   ├── 02_types_of_evals.ipynb
│   ├── 03_creating_eval_datasets.ipynb
│   ├── 04_building_evaluators.ipynb
│   ├── 05_running_evals_and_langsmith.ipynb
│   ├── 06_error_propagation_examples.ipynb
│   └── 07_final_project_end_to_end.ipynb
├── assets/
├── solutions/
├── requirements.txt
└── README.md
```

---

## 🛠️ Requirements

```
openai
langchain
langchain-core
langchain-openai
langgraph
langsmith
tiktoken
requests
jupyter
```

Install all with:
```bash
pip install -r requirements.txt
```

---

## 🎓 Learning Path

### Beginner
1. Start with **PART 1** - LLM basics
2. **PART 2** - Agent concepts
3. **PART 3** - Build agents

### Intermediate
4. **PART 4** - Add observability
5. **PART 5.1-2** - Understand evals

### Advanced
6. **PART 5.3-4** - Create datasets/evaluators
7. **PART 5.5-7** - Run evals + final project

---

## 🔗 Resources

- [LangSmith Docs](https://docs.smith.langchain.com)
- [LangChain Docs](https://python.langchain.com)
- [LangGraph Docs](https://langchain-ai.github.io/langgraph/)
- [OpenAI API](https://platform.openai.com)

---

## 📝 License

MIT License - Feel free to use!

---

## 🤝 Contributing

Issues and PRs welcome!

---

*Built with ❤️ for the AI developer community*