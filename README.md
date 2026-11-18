# Randyverse — Desktop AI Assistant

Release: **2.9.1** | build: **2026-10-06** | Python: **>=3.10, <3.14**

> Repository: https://github.com/metaverve/randyverse

## Overview

**Randyverse** is an open-source desktop AI assistant for `Linux`, `Windows` and `macOS`. It supports models from `OpenAI` (`GPT-6 Astra`, `GPT-5.6`, `GPT-4`, etc.), `Google Gemini`, `Anthropic Claude`, `xAI Grok`, `Perplexity / Sonar`, `DeepSeek`, plus models available through `HuggingFace`, `LlamaIndex`, OpenAI-compatible APIs, and local `Ollama` installations such as `DeepSeek`, `Qwen`, `gpt-oss`, `Gemma`, `Mistral`, `Llama`, and others.

Beyond chat, Randyverse includes Agents with Chat, Orchestrator and Swarm workflows, Agent Skills, plugins and MCP connectors, RAG, files and attachments, Python/IPython and system tools, web search, vision and camera input, image and video generation, Computer use, realtime voice, speech input/output, memory, automation, and external integrations. Models can use local and remote tools, work with files, call APIs, and control the desktop or browser when enabled.

## Features

- **Chat** with multiple model providers (OpenAI, Gemini, Claude, Grok, DeepSeek, Perplexity, Ollama, HuggingFace, OpenAI-compatible APIs)
- **Agents** — autonomous agents with Chat, Orchestrator and Swarm workflows, plus Agent Skills
- **Plugins & MCP** — built-in plugin system and Model Context Protocol connectors
- **RAG** — index and query your own documents and vector stores
- **Tools** — Python/IPython execution, system (OS) shell tool with sandboxed or Docker backends, web search, file handling
- **Vision** — image input, camera capture, inline image analysis
- **Image & video generation** — via supported providers
- **Voice** — realtime voice mode, speech recognition (STT) and speech synthesis (TTS)
- **Computer use** — let models control mouse/keyboard and browser when enabled
- **Memory, automation, scheduling** — persistent memory and task automation
- **Themes** — dark and light UI themes, customizable layout

## Installation

### From source

Requirements: Python **>=3.10, <3.14**

```bash
git clone https://github.com/metaverve/randyverse.git
cd randyverse
pip install -r requirements.txt
python run.py
```

Or with Poetry:

```bash
poetry install
poetry run python run.py
```

### As a package

```bash
pip install .
randyverse
```

## Configuration

On first launch, open **Config → Settings** and add an API key for your preferred provider (OpenAI, Anthropic, Google, xAI, DeepSeek, etc.). Local models via Ollama work without API keys.

User data and configuration are stored in the per-user Randyverse config directory (e.g. `~/.config/randyverse-net` on Linux).

## Running tests

```bash
./run-tests.sh
```

## Building

Build scripts for Windows installers, Linux packages and AppImage live in `bin/`. PyInstaller specs (`windows.spec`, `linux.spec`) and `AppImageBuilder.yml` are included at the repository root.

## Attribution

Randyverse is a white-label distribution of **[PyGPT](https://github.com/szczyglis-dev/py-gpt)** by Marcin Szczygliński, used under the terms of the MIT License. See `LICENSE` and `NOTICE` for details.

## License

MIT — see `LICENSE`.
