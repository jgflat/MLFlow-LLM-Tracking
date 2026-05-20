# MLflow LLM Tracking Project

## Overview
This project demonstrates how MLflow can be used to track and evaluate Large Language Model (LLM) interactions and performance metrics.

The notebook integrates OpenAI models with MLflow to monitor:
- prompts
- latency
- token usage
- experiment parameters
- model outputs

This project highlights practical LLMOps and experiment tracking workflows.

---

## Features
- OpenAI API integration
- MLflow experiment tracking
- Token usage monitoring
- Request latency tracking
- Prompt logging
- Automated experiment organization

---

## Technologies Used
- Python
- MLflow
- OpenAI API
- tiktoken
- dotenv

---

## How It Works

1. Multiple prompts are sent to an OpenAI model.
2. Responses are generated using GPT-4o-mini.
3. MLflow logs:
   - prompt text
   - model parameters
   - token counts
   - latency metrics
4. Results are stored as experiment runs for comparison and evaluation.

---

## Metrics Logged
- Request latency
- Prompt tokens
- Completion tokens
- Total tokens
- Request count

---

## Important Notes

### API Key Setup
Create a `.env` file:

```
OPENAI_API_KEY=your_api_key_here
```

Do NOT upload your `.env` file to GitHub.

---

### MLflow Server
This project uses a local MLflow tracking server:

```python
mlflow.set_tracking_uri("http://127.0.0.1:5000")
```

To run locally, start an MLflow server before executing the notebook.

Example:

```bash
mlflow ui
```

---

## Key Skills Demonstrated
- LLMOps workflows
- Experiment tracking
- AI performance monitoring
- API integration
- Token accounting
- Operational AI evaluation

---

## Files
- `mlflow_llm_tracking.ipynb` → main notebook
- `README.md` → project overview
- `requirements.txt` → dependencies

---

## Author
Jeremy Granflaten
