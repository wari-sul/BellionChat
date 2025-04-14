# BellionChat Overview
BellionChat is a web-based chat platform designed to simplify interactions with multiple AI model providers. It serves as a centralized hub for engaging with and exploring a diverse range of large language models (LLMs).

## Supported AI Model Providers
Below is a list of supported LLMs integrated into BellionChat, along with details on API access for each provider. Be sure to review the terms and conditions of each provider before starting.

| Provider            | Description                                                | Link to API Key                                                                 | Notes                                               |
|---------------------|------------------------------------------------------------|----------------------------------------------------------------------------------------|-----------------------------------------------------|
| 🌍 OpenAI          | Includes GPTs and more                                    | [Get Key](https://platform.openai.com/api-keys)                                | 💳 Paid                                             |
| ✨ Google Gemini   | Gemini models                                             | [Get Key](https://aistudio.google.com/app/apikey)                              | ✅ Free tier available                              |
| 🟨 Anthropic       | Claude models                                             | [Get Key](https://console.anthropic.com/settings/keys)                         | 💳 Paid                                             |
| 🌊 DeepSeek        | Competing with OpenAI’s leading models                    | [Get Key](https://platform.deepseek.com/api_keys)                              | ℹ️ Check website for pricing                       |
| 🐴 Ollama          | Open-source solution for running LLMs locally             | Not applicable (local setup)                                                  | 🛠️ Create your own AI universe!                    |
| 🎯 Cohere          | Command models                                            | [Get Key](https://dashboard.cohere.com/api-keys)                               | ✅ Free tier available                              |
| 🛫 Groq Inc.       | Built for rapid inference with open-source models         | [Get Key](https://console.groq.com/keys)                                       | ✅ Free tier available ⚡                           |
| ⚡ Cerebras         | Focused on high-speed inference                           | [Get Key](https://cloud.cerebras.ai/platform/)                                 | ✅ Free tier available 🛫                           |
| 💠 SambaNova       | Optimized for quick processing                            | [Get Key](https://cloud.sambanova.ai/apis)                                     | ✅ Free tier available                              |
| 🔄 OpenRouter      | Access point to all LLMs                                  | [Get Key](https://openrouter.ai/)                                             | ℹ️ Check website for pricing                       |
| 🌤️ Together AI    | The Cloud for AI Acceleration                             | [Get Key](https://api.together.ai/settings/api-keys)                           | ✅ Free for specific models                         |
| 📶 Deep Infra      | Robust AI infrastructure for scalability                  | [Get Key](https://deepinfra.com/)                                             | ℹ️ Check website for pricing                       |
| 🔥 Hyperbolic      | The Open Access AI Cloud                                  | [Get Key](https://app.hyperbolic.xyz/settings#api-key)                         | ℹ️ Check website for pricing                       |




## Screenshot
- **Light theme:**

*(TODO: Add Light Theme Screenshot)*

**Dark Theme:** 

*(TODO: Add Dark Theme Screenshot)*


With BellionChat, you can easily navigate and assess the strengths and limitations of different AI models through an intuitive,
user-friendly interface.

## Key Features

- 🖱️ Browser-Based - No installation needed ⚡
- ✅ Code Execution (Run code with Google Gemini)
- 🗨️ TTS - Realistic text-to-speech powered by ElevenLabs
- 🎧 STT - Speech-to-Text functionality with Groq/Whisper
- 🔄 Seamless integration with a variety of AI models
- 💫 Modern and intuitive web interface 🌎
- 🎨 Syntax highlighting for code blocks 🖌️
- 📤 One-click download for AI-generated code outputs
- 🛠️ Customizable system prompts for tailored responses 🔧
- 🌏 Special command for quick and easy language translation
- 📎 Upload various file types (text, PDF, images, video) to Google Gemini for analysis and processing
- 🧩 Awesome Prompts - Over 150 fantastic prompts, many sourced from [Awesome ChatGPT Prompts](https://github.com/f/awesome-chatgpt-prompts), selectable with just one click.



## API Key Management

Your API keys are stored locally using `localStorage`, and requests are sent directly to the official provider's API
(OpenAI, Anthropic, Google, Groq, Cerebras) without routing through any external proxy.

# Special Commands
Quickly perform actions using these special commands for enhanced functionality.

## Core Features
| Feature                          | Command Example                                      | Description                                                                 |
|----------------------------------|-----------------------------------------------------|-----------------------------------------------------------------------------|
| **Grounding with Google Search** | `g: What's the main news today?`                   | Enhances response accuracy and recency using Gemini API's internal RAG. Works with any Gemini 2.0 model (Flash or Pro). |
| **Deep Thinking (Claude 3.7 Sonnet)** | `dt: Explain quantum entanglement`            | Switch between standard and extended thinking modes with Claude 3.7 Sonnet. |
| **Translation**                  | `t:spanish Hello everyone!`                       | Easily translate text by specifying the target language. AI auto-detects the source language. Alternative: `translate:spanish`. |
| **YouTube Summary**              | `Summarize this video https://www.youtube.com/watch?v=r7pEdhnS3tI` | Summarize or ask questions about YouTube videos based on captions. Use larger context models like Google Gemini for best results. |
| **Retrieval-Augmented Generation (RAG)** | `s: What is the latest news?`              | Perform quick Google searches to retrieve relevant information. Alternative: `search:`. |

## Code Execution
| Feature                          | Command Example                                      | Description                                                                 |
|----------------------------------|-----------------------------------------------------|-----------------------------------------------------------------------------|
| **JavaScript in Browser**        | `js: How many R's in 'Strawberry'?`               | Execute AI-generated JavaScript code in your browser. Use with caution and review code before running. Alternative: `javascript:`. |
| **Python in Remote Environment** | `py: Run a python code to write "tseb eht sI noirO" in inverse order` | Execute Python code in Google's remote environment (only with Google Gemini). Returns code and output. |

## Keyboard Shortcuts
| Action                           | Shortcut                                            | Description                                                                 |
|----------------------------------|-----------------------------------------------------|-----------------------------------------------------------------------------|
| **Close Current Chat**           | `Ctrl + Q`                                         | Close the active chat and start a new one.                                  |
| **Toggle Theme**                 | `Shift + T`                                        | Switch between dark and light theme modes.                                  |

# How to Run
To run BellionChat first download this repository.

You can download it by running the following command in your terminal:

```bash
git clone https://github.com/wari-sul/BellionChat.git
```
Or download the zip file from the repository by clicking on the green button "Code" and then [Download ZIP]

After downloading, just open the folder and click on index.html if you don't have a server.
If you do, just access the directory where the project was saved. It's that simple.


# Google CSE API Key
*This will be useful when you are not using Google's Gemini models, as the ``g:`` command will not work.

Sometimes you might want AI to search the web and respond based on that information.


To allow AI to search using Google, you will need Google CSE (Custom Search Engine) API Key and CX.
- First, create a custom search here [Google CSE Panel](https://programmablesearchengine.google.com/controlpanel/all)
- Copy your CX ID
# Setup and Configuration for BellionChat
Follow these concise instructions to set up and run BellionChat with additional features.

## How to Run
1. **Download the Repository**:
   - Clone using the terminal:
     ```bash
     git clone https://github.com/wari-sul/BellionChat.git
     ```
   - Or download the ZIP file from the repository by clicking the green "Code" button and selecting [Download ZIP].
2. **Run the Application**:
   - Open the folder and click `index.html` if you don’t have a server.
   - If using a server, access the directory where the project is saved.

## Google CSE API Key (For Web Search)
*Useful when not using Google Gemini models, as the `g:` command won't work.*

To enable AI web search with Google:
1. Create a custom search at [Google CSE Panel](https://programmablesearchengine.google.com/controlpanel/all) and copy your CX ID.
2. Get your API Key at [Google Developers](https://developers.google.com/custom-search/v1/introduction) by clicking *Get a Key*.
3. Configure in BellionChat: Go to `Options` -> `More Options`, and enter your CX ID and API Key.
4. Use the feature by starting prompts with `s:`, e.g., `s: What's today's news?`
   - *Note*: Results may be snippets with limited context. Consider the RAG Endpoint solution below for better results.

## RAG Endpoint (Enhanced Search Results)
For improved search functionality:
1. Set up a compatible RAG endpoint (instructions pending - TODO).
2. Configure in BellionChat: Go to `Options` -> `Advanced`, enter the RAG endpoint URL, and click `Activate`.
3. Use by starting prompts with `s:`, e.g., `s: What's the news today?` AI will search and respond based on web data.

## CORS Handling (For SambaNova)
To bypass CORS errors when using SambaNova:
- API requests are routed through `cors-proxy.php`, which forwards them to the platform.
- *Note*: This does not hide your IP; it only forwards the request, as direct browser requests via JavaScript are restricted.

## YouTube Caption Integration
To ask about or summarize YouTube video content:
1. Set up a compatible YouTube subtitle downloading service (instructions pending - TODO).
   - Can be hosted on localhost or a remote server.
2. Configure in BellionChat: Go to `Options` -> `YouTube Captions`, and enter the service URL, e.g., `http://localhost/YoutubeSubtitlesDownloader/`.
3. Share a YouTube URL in the chat to query or summarize video content.

---

# Future Works (BellionAPI Implementation)

Below is a structured overview of the planned enhancements for BellionChat, including the implementation of a backend API for secure, authenticated access to specific LLM models. 

## Backend Development (BellionAPI-Worker Repo)
| Feature                  | Description                                                                 |
|--------------------------|-----------------------------------------------------------------------------|
| **Backend Service**      | Develop a new backend using Hono framework on Cloudflare Workers with API endpoints (e.g., `/api/proxy/llm`, `/api/user/profile`). |
| **Authentication (Auth0)** | Configure Auth0 for user login/signup, implement JWT verification middleware, and define an "admin" role for bypassing rate limits. |
| **Database (Supabase)**  | Set up a Supabase project for user data storage and integrate Supabase client/API with the backend. |
| **LLM Proxy**            | Store Groq/OpenRouter API keys securely in Worker secrets, implement request forwarding logic in `/api/proxy/llm`, and handle streaming responses. |
| **Rate Limiting (Cloudflare)** | Configure Cloudflare Rate Limiting rules for API endpoints with bypass logic for admin users. |
| **Secure API Key Storage** | Implement robust mechanisms for securely storing and managing LLM API keys in the backend. |

## Frontend Development (BellionChat Repo)
| Feature                  | Description                                                                 |
|--------------------------|-----------------------------------------------------------------------------|
| **Frontend Integration** | Integrate Auth0 SPA SDK for login/logout UI and token management, update model list to include "BellionAPI" models, and modify chat logic to call backend API for proxied models when logged in. |
| **Frontend Rewrite**     | Refactor using React and twin.macro (Tailwind CSS-in-JS) for better component structure, maintainability, and styling. |

## Deployment Strategies
| Feature                  | Description                                                                 |
|--------------------------|-----------------------------------------------------------------------------|
| **Cloudflare Deployment**| Deploy backend to Cloudflare Workers and frontend to Cloudflare Pages, configuring all necessary environment variables and secrets. |
| **Vercel Deployment**    | Add configuration and documentation for one-click deployment to Vercel as an alternative or complement to Cloudflare. |
| **Dockerization**        | Create Docker configurations for easier local development and potential alternative deployment strategies for backend/frontend. |

## Additional Enhancements
| Feature                  | Description                                                                 |
|--------------------------|-----------------------------------------------------------------------------|
| **Enhanced Database Integration** | Expand Supabase usage beyond authentication to store user preferences, chat history, or other application data. |
| **Expanded Authentication** | Build on Auth0 integration with features like social logins and additional user roles. |
