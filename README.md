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


> The repo is intentionally “learning-first”: small experiments, comparisons, and iterative improvements.

---

### Skills & techniques practiced ###

# 1. OpenAI API (Small Experiments)

This folder contains small experiments where I interact with an LLM through an API and test prompt behavior in a more repeatable way than chat.

## What I’m practicing

- Minimal request/response loops
- Separating **prompt text** from **code**
- Running the same prompt with small variations
- Capturing outputs to compare versions

# 2. LLM Fundamentals (Behavior & Limits)

This folder is about understanding **how LLMs behave** so prompting becomes less “guessing” and more “engineering”.

## What I’m testing here

- Tokens / context windows: what changes when context grows
- Ambiguity: how models choose an interpretation
- Hallucinations: when the model confidently invents details
- Instruction hierarchy: how system/user context affects outputs
- Robustness: how outputs change with small wording differences

## Outcome

The goal is not theory—it's *practical intuition*:
- when to add constraints
- when to add examples
- when to ask the model to state assumptions
- when to simplify the task

# 3. Core Techniques (Applied Prompting)

This folder holds *hands-on* work around prompt engineering techniques: turning vague requests into predictable outputs.

## What I practice here

- **Clarity & specificity**: remove ambiguity, define success criteria
- **Constraints**: limit scope, style, length, and “don’t do X”
- **Structured outputs**: templates, tables, JSON-like schemas
- **Few-shot examples**: show the model what “good” looks like
- **Iteration**: quick prompt versions with measurable improvements

---

## Getting started (local)

## Clone
```bash
git clone https://github.com/ghirageorge/AI_Prompt_Engineering.git
cd AI_Prompt_Engineering
```

## How I run this locally (optional)

```bash
python -m venv .venv
# Windows PowerShell:
#   .\.venv\Scripts\Activate.ps1
# macOS/Linux:
#   source .venv/bin/activate

pip install -r req.txt
pip install jupyter
jupyter lab
```