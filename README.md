# AI Prompt Engineering (Course Notes + Hands-on Exercises)

This repository is my learning log and practice workspace for an AI Prompt Engineering course.  
It contains **Jupyter notebooks** and small exercises where I experiment with prompting patterns, LLM fundamentals, and basic API usage. 

---

## What’s inside

High-level structure (folders may grow as I progress):

- **`llm-fundamentals/`**
  - Notes + exercises about how LLMs behave (tokens, context limits, ambiguity, hallucinations, etc.)
- **`Core-techniques/`**
  - Practical prompting techniques and reusable patterns
- **`openai-api/`**
  - API-oriented experiments (calling an LLM, controlling outputs, iterating on prompts)
- **`req.txt`**
  - Python dependencies list 

> The repo is intentionally “learning-first”: small experiments, comparisons, and iterative improvements.

---

## Skills & techniques practiced

### Prompting fundamentals
- Writing clear instructions: goal, constraints, and “what good looks like”
- Providing context without overloading the model
- Asking for assumptions and edge cases when requirements are unclear
- Controlling verbosity and tone

### Core prompt engineering patterns
- **Zero-shot vs. few-shot** prompting (using examples to shape outputs)
- **Role prompting** (giving the model a specific job/persona)
- **Structured outputs** (JSON / bullet formats / templates)
- **Decomposition** (breaking a task into steps or sub-tasks)
- **Self-checking** prompts (ask the model to verify requirements or validate outputs)

### Practical workflow habits
- Iterating on prompts with small, measurable changes
- Keeping “prompt versions” and documenting what changed + why
- Creating reusable prompt templates for common tasks

### API basics (where applicable)
- Loading environment variables safely (never committing secrets)
- Simple request/response loops for experimentation
- Comparing outputs across prompt variants

---

## Getting started (local)

### 1) Clone
```bash
git clone https://github.com/ghirageorge/AI_Prompt_Engineering.git
cd AI_Prompt_Engineering
