# Api_for_chatgpt_llm
# NVIDIA API Chat Completion Script

This repository contains a simple Python script demonstrating how to use the `openai` SDK to interact with large language models hosted via the **NVIDIA API Catalog** (using the `integrate.api.nvidia.com` endpoint).

## Prerequisites

Before running the script, ensure you have the required dependencies installed:

```bash
pip install openai
```

## How to Use the Code

1. **Obtain an API Key**: Sign up or log into the [NVIDIA API Catalog](https://build.nvidia.com/) to obtain your personal NVIDIA API key.
2. **Configure the Client**: Replace the placeholder string in the `api_key` parameter with your actual NVIDIA API key.
3. **Run the Script**: Execute the script using Python:
   ```bash
   python script.py
   ```

## Where to Give Input

You can customize the script's behavior by modifying the following parameters directly in the code:

* **Target Prompt / Question**: Change the text inside the `"content"` key of the `messages` list to ask a different question.
  ```python
  messages=[{"content": "YOUR_QUESTION_HERE", "role": "user"}]
  ```
* **Model Selection**: Change the `model` parameter string to target any other supported LLM available in the NVIDIA catalog (e.g., `meta/llama-3.1-405b-instruct`).
* **Generation Settings**: Adjust parameters like `temperature` (creativity level), `top_p` (nucleus sampling), or `max_tokens` (maximum output length) based on your performance needs.
