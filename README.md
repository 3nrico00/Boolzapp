# Boolzap

**Chatting with an AI agent through a mock WhatsApp web interface**

Boolzap is a simple front-end experiment that simulates a WhatsApp Web–style chat to talk with an AI bot (Gemini 2.5 Flash), called **Silv-IA**.  
The interface is entirely client-side and was created mainly as a learning exercise, not as a production-ready web application.

## Project goals

The main goal of this project is to **broaden my personal knowledge** in areas beyond my usual work, rather than becoming a professional web developer.  
I strongly believe that any additional skill or concept can be useful in the future, so this repo is part of that ongoing learning path.

This project was built step by step by following the lessons of the **“Boolean Coding Week”**, and all content (UI labels, prompts, comments) is primarily in **Italian**.

## Project structure

The repository contains three files, which together implement the front-end of the mock WhatsApp web page:

- `index.html` – The main HTML file. Opening this file in a browser loads the mock WhatsApp-style interface and allows you to chat with Silv-IA.
- `style.jss` – The stylesheet that defines the layout, colors, and general look of the mock WhatsApp interface.
- `script.js` – The JavaScript logic that:
  - Handles user input and message rendering.
  - Sends requests to the Gemini 2.5 Flash model.
  - Displays AI responses in the chat window.

There is **no back-end** component: everything runs in the browser.

## Language and system prompt

By default, the project is configured to chat with Silv-IA in **Italian**.

- To chat in Italian: simply open `index.html` in your browser after setting the API key (see below).
- To chat in English: change the value of the **`systemPrompt`** variable in `script.js` to an English prompt that defines the behavior and style of the AI.

Example idea (you will customize it directly in `script.js`):
_`const systemPrompt = "You are Silv-IA, an AI assistant that answers in English with clear and concise messages.";`_


## ⚠️ API key required (must-read)

To actually talk with the AI (Gemini 2.5 Flash), you **must** provide a valid API key from Google AI Studio.

1. Go to:  
   https://aistudio.google.com/api-keys
2. Create or retrieve an API key for **Gemini 2.5 Flash**.
3. Open `script.js`.
4. Locate the variable named **`keyNumber`**.
5. Set your API key as the value of `keyNumber`, for example:
   _`const keyNumber = "YOUR_API_KEY_HERE"`_

   
> **IMPORTANT:**  
> - The project **will not work** without a valid API key in `script.js`.  
> - Never commit or publish your real API key in a public repository.  
>   Consider using environment variables or a private configuration in more advanced setups.

## How to run the project

1. Clone or download this repository.
2. Open `script.js` and set your API key in the `keyNumber` variable.
3. Save the file.
4. Open `index.html` in your browser (double-click or drag-and-drop into the browser window).
5. Start chatting with **Silv-IA** in the mock WhatsApp interface.

No additional build steps or dependencies are required: it is a pure HTML/CSS/JS front-end.

## Limitations and disclaimer

- The project is **not fault-proof** and is **not** intended for production use.
- Error handling, security, and edge cases are minimal or simplified.
- The interface and code were written for **learning purposes**, so the structure may not reflect best practices used in professional applications.

Use this repository as a small sandbox to explore how to:

- Build a simple chat UI in the browser.
- Connect a front-end to a modern LLM (Gemini 2.5 Flash) via API.
- Experiment with prompts, languages, and interface tweaks.

## Credits

- Project name: **Boolzap**
- Description: *Chatting with an AI agent through a mock WhatsApp web interface*
- Built as a personal learning project, following the **“Boolean Coding Week”** lessons.
- AI model: **Gemini 2.5 Flash** (via Google AI Studio API).
- Chatbot persona: **Silv-IA**.
