# Paris Tour Guide Mini Chatbot

**Peterman Reality Tours**

## Overview

This project is an AI-powered travel guide developed for **Peterman Reality Tours**, an internationally acclaimed tourism company. It leverages **OpenAI’s API** to create an intelligent chatbot that acts as a virtual Parisian expert, capable of answering common tourist questions with accuracy, clarity, and cultural insight.

The goal is to enhance the travel planning experience by providing users with reliable, well-informed responses about Paris’s iconic landmarks and must-see attractions—making exploration more engaging even before arriving in the city.

---

## Project Objective

The primary objective of this project is to build a **user-friendly AI chatbot** that:

* Responds intelligently to predefined Paris-related travel questions
* Provides concise yet informative answers
* Simulates the expertise of a local Parisian travel guide
* Enhances customer engagement for Peterman Reality Tours

The chatbot maintains conversational context by storing all questions and responses in a structured conversation history.

---

## How It Works

The chatbot uses a list of dictionaries called `conversation`, where each entry contains:

* **role** – Identifies the speaker (`system`, `user`, or `assistant`)
* **content** – The message text

The conversation always begins with a **system message** that defines the chatbot’s behavior as a professional Paris travel guide.

Model configuration:

* **Model:** `gpt-4o-mini`
* **Temperature:** `0.0` (deterministic and factual responses)
* **Max Tokens:** `100` (concise outputs)

---

## Supported Tourist Questions

The chatbot is designed to answer the following questions:

1. How far away is the Louvre from the Eiffel Tower (in miles) if you are driving?
2. Where is the Arc de Triomphe?
3. What are the must-see artworks at the Louvre Museum?

Each question and its corresponding AI-generated response are appended to the conversation history to preserve context.

---

## OpenAI API Key Setup

To run this project, you must provide **your own OpenAI API key**.

The recommended approach is to store your API key as an environment variable:

### macOS / Linux

```bash
export OPENAI_API_KEY="your_api_key_here"
```

### Windows (PowerShell)

```powershell
setx OPENAI_API_KEY "your_api_key_here"
```

The `OpenAI()` client automatically reads this environment variable. If needed, users may modify the client initialization to manage custom configurations or multiple API keys.

---

## Customization

You can easily adapt this project by:

* Updating the **system prompt** to change the chatbot’s role or personality
* Replacing Paris-related questions with other cities or domains
* Adjusting temperature or token limits for different response styles
* Expanding the conversation for more complex interactions

---

## Use Cases

* Virtual travel assistants
* Tourism and hospitality chatbots
* Educational demos for OpenAI API usage
* AI-powered customer engagement tools

---

## 🏁 Conclusion

This project demonstrates a practical and professional application of OpenAI’s API to build a context-aware AI travel assistant. By combining structured conversation design with deterministic model settings, it delivers reliable, engaging, and high-quality travel guidance suitable for real-world tourism platforms.
