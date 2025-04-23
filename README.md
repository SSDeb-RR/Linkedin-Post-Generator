# AI Based LinkedIn Post Generator

Fine-tuned LLama 3.3 (7B) versatile model using Langchain and Groq Console on LinkedIn post data of an influencer. Utilized Chain-of-Thought Prompting to design more effective prompt templates and extract metadata from raw post data. Developed a basic UI front-end using Streamlit for seamless interaction with the tool.

---

## 🧠 Project Overview

This tool helps LinkedIn influencers like **Akshat** automate and personalize content creation. By feeding in past posts, the tool extracts key metadata like topic, tone, and length, and uses this to generate new posts aligned with the influencer’s unique voice.

---

## 🧱 Technical Architecture

### **Stage 1: Metadata Extraction**
- Input raw LinkedIn post data.
- Extracts structured metadata such as:
  - **Topic**
  - **Language**
  - **Length**

### **Stage 2: AI Post Generation**
- User selects:
  - Desired **topic**
  - Preferred **language**
  - Required **post length**
- A few relevant past posts are fetched and used for **few-shot prompting**.
- LLama 3.3 model generates a new post consistent with the influencer’s style.

---

## ✨ Features

- ✅ Automatically extracts key metadata from past posts.
- ✅ Few-shot style learning to match user's writing tone.
- ✅ Multilingual post generation support.
- ✅ User-controlled post length (short, medium, long).
- ✅ Streamlit-based UI for interactive post creation.
- ✅ Chain-of-Thought prompting for better metadata understanding.

---

## 🛠️ Tech Stack

- **LLama 3.3 (7B)** — Fine-tuned LLM for post generation.
- **Langchain** — Chains logic and prompts in a modular fashion.
- **Groq Console** — High-performance inference backend.
- **Streamlit** — Lightweight front-end for easy UI.
- **Python** — Core programming language.
- **Chain-of-Thought Prompting** — Structured reasoning behind prompt design.

---

## Set-up
1. To get started we first need to get an API_KEY from here: https://console.groq.com/keys. Inside `.env` update the value of `GROQ_API_KEY` with the API_KEY you created. 
2. To get started, first install the dependencies using:
    ```commandline
     pip install -r requirements.txt
    ```
3. Run the streamlit app:
   ```commandline
   streamlit run main.py
   ```
