# asap.it

Welcome to asap.it, an AI-powered full-stack web development platform that lets you choose your preferred LLM for each prompt. Currently supports OpenAI, Anthropic, Ollama, OpenRouter, Gemini, LMStudio, Mistral, xAI, HuggingFace, DeepSeek, and Groq models.

## Features

- Full-stack development in the browser
- Multiple LLM support
- Package installation and management
- Node.js server capabilities
- Terminal access
- Project deployment
- File synchronization
- GitHub integration
- Docker support

## Quick Start

1. Install Git and Node.js
2. Clone the repository
3. Rename `.env.example` to `.env.local` and add your LLM API keys
4. Install dependencies:

```bash
pnpm install
```

## Development

Run the development server:

```bash
pnpm run dev
```

## Docker Support

Build and run with Docker:

```bash
# Development
npm run dockerbuild
docker-compose --profile development up

# Production
npm run dockerbuild:prod
docker-compose --profile production up
```

## Environment Variables

Required (set only the ones you plan to use):

```
GROQ_API_KEY=XXX
OPENAI_API_KEY=XXX
ANTHROPIC_API_KEY=XXX
```

Optional:

```
VITE_LOG_LEVEL=debug
OLLAMA_API_BASE_URL=http://localhost:11434
DEFAULT_NUM_CTX=8192
```
