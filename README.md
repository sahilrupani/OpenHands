# OpenHands Coding Agent — Railway Template

![OpenHands](https://opengraph.githubassets.com/4a3fa291732195ae8467266dd5a49902a29d66a2efa92dcdd854c9c7a7e035f3/OpenHands/OpenHands)

> Self-hosted, open-source autonomous AI coding agent. Bring your own LLM. Full autonomy.

[![Deploy on Railway](https://railway.com/button.svg)](https://railway.com/deploy/openhands-coding-agent?utm_medium=integration&utm_source=button&utm_campaign=openhands-coding-agent)

---

## What is OpenHands?

OpenHands is an open-source, model-agnostic platform for autonomous AI software development. Unlike coding assistants that suggest snippets, OpenHands runs agents that **plan, write, debug, and apply changes** across your entire codebase — end to end — without handholding.

Trusted by engineering teams at AMD, Google, Amazon, Netflix, and NVIDIA. Backed by 60,000+ GitHub stars and an $18.8M Series A.

![OpenHands Dashboard](https://res.cloudinary.com/asset-cloudinary/image/upload/v1776595971/openhands_dashboard_ltl7nw.png)

---

## Deploy on Railway in One Click

[![Deploy on Railway](https://railway.com/button.svg)](https://railway.com/deploy/openhands-coding-agent?utm_medium=integration&utm_source=button&utm_campaign=openhands-coding-agent)

This Railway template gives you a fully hosted OpenHands instance with:

- **Browser-accessible web UI** — interact with your AI engineer from any device
- **Persistent workspace volume** — agent state, files, and config survive restarts
- **Any LLM you choose** — Claude, GPT-4o, Gemini, DeepSeek, Llama via Ollama, or any OpenAI-compatible endpoint
- **Sandboxed Docker runtime** — agents execute in isolation; your host is never touched
- **Auto-restart on crash** — service recovers automatically from failures
- **Full audit trail** — every action, file change, and command is logged in the UI

---

## Getting Started

### 1. Deploy to Railway

Click the button above or go to [railway.com/deploy/openhands-coding-agent](https://railway.com/deploy/openhands-coding-agent).

### 2. Set Your Environment Variables

After deployment, configure the following in your Railway service settings:

```bash
SANDBOX_RUNTIME_CONTAINER_IMAGE=docker.all-hands.dev/all-hands-ai/runtime:0.17-nikolaik
LLM_MODEL=claude-sonnet-4-20250514   # or your preferred model
LLM_API_KEY=your_api_key_here
LOG_ALL_EVENTS=true
```

### 3. Open the Web UI

Visit your Railway public URL. The OpenHands interface will load in your browser. Go to **Settings → Language Models** to confirm your LLM configuration.

### 4. Run Your First Task

Type a plain-English instruction and let the agent execute it:

```
Fix the failing test in auth/login.py and open a pull request.
```

OpenHands will plan the fix, edit the file, run the tests, and commit the result.

---

## Common Use Cases

- **Autonomous bug fixing** — assign issues or failing tests to the agent and get production-ready PRs back
- **Codebase refactoring** — automate dependency upgrades, lint fixes, and legacy refactors across repositories
- **Full-stack feature development** — describe a feature in plain English and let the agent scaffold, implement, and test it

---

## OpenHands vs. Alternatives

| | OpenHands | Devin | GitHub Copilot Agent | Claude Code |
|---|---|---|---|---|
| **Open source** | ✅ MIT | ❌ | ❌ | ❌ |
| **Self-hostable** | ✅ | ❌ | ❌ | ❌ |
| **Model agnostic** | ✅ Any LLM | ❌ | ⚠️ Curated | ❌ Anthropic only |
| **Pricing** | Free (BYO key) | ~$500/mo | $10–$39/mo | Usage-based |
| **Browser automation** | ✅ | ✅ | ❌ | ❌ |
| **Self-hosted on Railway** | ✅ | ❌ | ❌ | ❌ |

---

## Resources

- [OpenHands GitHub Repository](https://github.com/OpenHands/OpenHands)
- [OpenHands Documentation](https://docs.all-hands.dev)
- [Supported LLM Providers](https://docs.all-hands.dev/usage/llms/llms)
- [Railway Template Page](https://railway.com/deploy/openhands-coding-agent)
- [OpenHands Docker Image](https://hub.docker.com/r/all-hands-ai/openhands)

---

## About Railway

Railway is a full-stack cloud platform for deploying web apps, servers, databases, and AI agents — with automatic scaling, private networking, persistent volumes, and real-time observability. Deploy OpenHands in one click and get a self-hosted autonomous AI engineer with zero infrastructure overhead.

[![Deploy on Railway](https://railway.com/button.svg)](https://railway.com/deploy/openhands-coding-agent?utm_medium=integration&utm_source=button&utm_campaign=openhands-coding-agent)
