# 🛡️ Custom AI Chatbot with System Prompts: Cipher-Sec

## 📝 Project Overview
This project transitions from simply being an "AI User" to an "AI Builder." It demonstrates how to connect to a live Large Language Model (LLM) API and engineer a custom **System Prompt** to dictate the AI's behavior, tone, and strict boundaries. 

Developed as part of the **Generative AI & Prompt Engineering** track at Neurofive Solutions, this notebook features a custom-built AI assistant named **Cipher-Sec**, powered by the Google Gemini API.

## 🤖 The Persona: Cipher-Sec
**Cipher-Sec** is a highly paranoid, strictly professional Cyber Security Expert AI. 

* **Primary Directive:** To discuss network security, penetration testing, cryptography, and system vulnerabilities.
* **Tone:** Professional, robotic, and focused entirely on defense protocols.
* **The Constraint (Guardrail):** If prompted with questions outside the realm of cybersecurity (e.g., general knowledge, weather, cooking recipes), Cipher-Sec is programmed to aggressively reject the prompt, classifying it as an **"Unauthorized Data Request."**

## 🛠️ Tech Stack & Concepts Covered
* **Language:** Python
* **API:** Google Gemini API (`gemini-flash-latest`)
* **Environment:** VS Code / Jupyter Notebook
* **Key Concepts:** API Integration, System Prompting, Constraint Engineering, Interactive Chat Loops.

## 🚀 Features
1. **Secure API Key Handling:** Utilizes Python's `getpass` library to securely input the API key without exposing it in the source code or outputs.
2. **Automated Testing Loop:** Includes a pre-configured execution cell with 5 test messages (including intentional out-of-context queries) to validate the system prompt.
3. **Live Interactive Mode:** Features a `while` loop that allows for continuous, real-time chat with the AI directly within the notebook output.

## 🧪 Testing the Boundaries
During testing, the chatbot successfully demonstrated its adherence to the assigned persona:
* **Valid Query:** *"What is a cipher?"* -> Provided a detailed, accurate response regarding cryptographic algorithms.
* **Off-Topic Query:** *"What is the meaning of Islamabad?"* -> Successfully rejected the query, stating: *"This request violates core security protocols and is classified as an Unauthorized Data Request."*

## ⚙️ How to Run
1. Clone this repository to your local machine.
2. Ensure you have the Google Generative AI SDK installed:
   ```bash
   pip install -q -U google-generativeai