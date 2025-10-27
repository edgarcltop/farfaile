# FarfalleUp

Open-source AI-powered search engine.
Run local LLMs (**llama3**, **gemma**, **mistral**, **phi3**) &  custom LLMs through **LiteLLM**

## 📖 Overview
- 🛠️ [Tech Stack](#%EF%B8%8F-tech-stack)
- 🏃🏿‍♂️ [Getting Started](#%EF%B8%8F-getting-started)

## 🛠️ Tech Stack
- Frontend: [Next.js](https://nextjs.org/)
- Backend: [FastAPI](https://fastapi.tiangolo.com/)
- Search API: [SearXNG](https://github.com/searxng/searxng), [Tavily](https://tavily.com/), [Serper](https://serper.dev/), [Bing](https://www.microsoft.com/en-us/bing/apis/bing-web-search-api)
- Logging: [Logfire](https://pydantic.dev/logfire)
- Rate Limiting: [Redis](https://redis.io/)
- Components: [shadcn/ui](https://ui.shadcn.com/)

## Features
- Search with multiple search providers (Tavily, Searxng, Serper, Bing)
- Answer questions with cloud models (OpenAI/gpt4-o, OpenAI/gpt3.5-turbo, Groq/Llama3)
- Answer questions with local models (llama3, mistral, gemma, phi3)

## 🏃🏿‍♂️ Getting Started Locally
### Quick Start:
```
git clone https://github.com/edgarcltop/farfilleUp.git
cd farfilleUp && cp .env-template .env
```
Modify .env with your API keys (Optional, not required if using Ollama)

Start the app:
```
docker-compose -f docker-compose.dev.yaml up -d
```

Wait for the app to start then visit [http://localhost:3000](http://localhost:3000).

For custom setup instructions, see [custom-setup-instructions.md](/custom-setup-instructions.md)

## 🚀 Deploy

### Backend
After the backend is deployed, copy the web service URL to your clipboard.

### Frontend

Use the copied backend URL in the `NEXT_PUBLIC_API_URL` environment variable when deploying with Vercel.

[![Deploy with Vercel](https://vercel.com/button)](https://vercel.com/new/clone?repository-url=https%3A%2F%2Fgithub.com%2Frashadphz%2Ffarfalle&env=NEXT_PUBLIC_API_URL&envDescription=URL%20for%20your%20backend%20application.%20For%20backends%20deployed%20with%20Render%2C%20the%20URL%20will%20look%20like%20this%3A%20https%3A%2F%2F%5Bsome-hostname%5D.onrender.com&root-directory=src%2Ffrontend)

And you're done! 🥳

