# task-4
# General Health Query Chatbot

## 📌 Task Objective
The goal of this project is to develop a **safe, general health query chatbot** that can answer non-urgent, factual health-related questions.  
The chatbot uses an **OpenAI-compatible LLM API** (Anthropic Claude in this implementation) and includes safety filtering to block sensitive or emergency-related requests.  
It is designed for **educational purposes only** and always reminds users to consult qualified healthcare professionals.

---

## 📂 Dataset Used
No traditional dataset is used for training — the chatbot leverages **pre-trained large language models** via API.  
However, the safety filter uses a small **manually curated keyword list** to detect unsafe or urgent topics.

---

## 🤖 Models Applied
- **Claude 3.5 Sonnet (2024-10-22)** from Anthropic  
  - API: `anthropic` Python SDK  
  - Prompt engineering to provide clear, safe, and friendly answers.  
- Safety filter logic in Python to handle potentially dangerous inputs before sending them to the model.

---

## 📊 Key Results and Findings
- The chatbot successfully answers common, safe health questions such as:
  - “What are the symptoms of vitamin D deficiency?”
  - “How much water should an adult drink daily?”
  - “What foods are rich in iron?”
- Dangerous or emergency-related queries trigger a **warning response** rather than model interaction.
- The switch from OpenAI to Claude API eliminated quota issues for users with an Anthropic API key.
- Prompt design significantly influences the clarity and safety of responses.

---

## ⚠️ Disclaimer
This chatbot is **not** a replacement for professional medical advice.  
Always consult a qualified healthcare provider for diagnosis, treatment, or urgent concerns.
