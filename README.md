# Awesome Local AI Workstation

A practical map of local-first AI tools for developers: model runtimes, chat UIs, coding agents, commit helpers, speech tools, note assistants, and desktop companions.

This is not a benchmark list. It is a workstation list: what to install, what each tool is good at, and how the pieces fit together on a real laptop or desktop.

[![Validate catalog](https://github.com/StaryMoon/awesome-local-ai-workstation/actions/workflows/validate.yml/badge.svg)](https://github.com/StaryMoon/awesome-local-ai-workstation/actions/workflows/validate.yml)

Setup recipes: [docs/workstation-stacks.md](docs/workstation-stacks.md)

## Fast Stack

If you want a clean local AI workstation, start here:

| Layer | Pick |
|---|---|
| Model runtime | [Ollama](https://github.com/ollama/ollama), [llama.cpp](https://github.com/ggml-org/llama.cpp), [LocalAI](https://github.com/mudler/LocalAI) |
| Chat / web UI | [Open WebUI](https://github.com/open-webui/open-webui), [Jan](https://github.com/janhq/jan), [AnythingLLM](https://github.com/Mintplex-Labs/anything-llm) |
| Coding assistant | [Continue](https://github.com/continuedev/continue), [aider](https://github.com/Aider-AI/aider), [Open Interpreter](https://github.com/OpenInterpreter/open-interpreter), [Tabby](https://github.com/TabbyML/tabby) |
| Speech / audio | [whisper.cpp](https://github.com/ggml-org/whisper.cpp), [Qwen3ASRDemo](https://github.com/yumiaura/Qwen3ASRDemo) |
| Image / visual workflow | [ComfyUI](https://github.com/comfyanonymous/ComfyUI), [stable-diffusion-webui](https://github.com/AUTOMATIC1111/stable-diffusion-webui) |
| Notes / personal knowledge | [Khoj](https://github.com/khoj-ai/khoj), [Obsidian Copilot](https://github.com/logancyang/obsidian-copilot) |
| Small utilities | [AICommit](https://github.com/yumiaura/AICommit), [vibe-trading-bot](https://github.com/StaryMoon/vibe-trading-bot), [DailyDesk](https://github.com/StaryMoon/DailyDesk) |

## Catalog

### Runtimes

| Project | Use case | Notes |
|---|---|---|
| [Ollama](https://github.com/ollama/ollama) | Local model serving | Simple model pull/run workflow, widely supported by local tools. |
| [llama.cpp](https://github.com/ggml-org/llama.cpp) | Low-level inference | Fast C/C++ inference for GGUF models and CPU/GPU experiments. |
| [LocalAI](https://github.com/mudler/LocalAI) | OpenAI-compatible local API | Drop-in local API server for multiple model families. |
| [GPT4All](https://github.com/nomic-ai/gpt4all) | Local chat app and runtime | Friendly desktop entry point for local models. |
| [vLLM](https://github.com/vllm-project/vllm) | Local/high-throughput serving | Production-oriented LLM serving engine with OpenAI-compatible endpoints. |
| [LMDeploy](https://github.com/InternLM/lmdeploy) | Local model serving | Inference and deployment toolkit for LLMs and VLMs. |

### Chat and Workbench UIs

| Project | Use case | Notes |
|---|---|---|
| [Open WebUI](https://github.com/open-webui/open-webui) | Browser chat UI | Popular local web UI for Ollama and OpenAI-compatible backends. |
| [Jan](https://github.com/janhq/jan) | Desktop AI app | Local-first desktop app for running and chatting with models. |
| [AnythingLLM](https://github.com/Mintplex-Labs/anything-llm) | Knowledge base assistant | Local/private RAG workspace for documents and team knowledge. |
| [LibreChat](https://github.com/danny-avila/LibreChat) | Multi-provider chat UI | Useful when mixing local and cloud providers. |
| [Lobe Chat](https://github.com/lobehub/lobe-chat) | Multi-provider chat UI | Polished chat UI that can connect to local and remote model providers. |

### Coding Assistants

| Project | Use case | Notes |
|---|---|---|
| [Continue](https://github.com/continuedev/continue) | IDE assistant | VS Code / JetBrains assistant that can use local models. |
| [aider](https://github.com/Aider-AI/aider) | Git-aware coding agent | Terminal coding assistant that edits files through Git context. |
| [Open Interpreter](https://github.com/OpenInterpreter/open-interpreter) | Computer-use style assistant | Local code execution and computer-control style workflows. |
| [Tabby](https://github.com/TabbyML/tabby) | Self-hosted code completion | Local coding assistant server for teams and personal use. |
| [AICommit](https://github.com/yumiaura/AICommit) | Commit messages | Offline AI commit messages with Ollama / llama.cpp backends. |
| [Cline](https://github.com/cline/cline) | Agentic IDE workflow | VS Code coding agent that can work with local and remote model providers. |
| [Roo Code](https://github.com/RooVetGit/Roo-Code) | Agentic IDE workflow | Agentic coding extension with multi-mode workflows. |

### Speech, Audio, and Media

| Project | Use case | Notes |
|---|---|---|
| [whisper.cpp](https://github.com/ggml-org/whisper.cpp) | Local speech recognition | Lightweight local ASR using Whisper models. |
| [Qwen3ASRDemo](https://github.com/yumiaura/Qwen3ASRDemo) | Live microphone ASR | Demo for live microphone recognition with Qwen3-ASR. |
| [SubForge](https://github.com/yumiaura/SubForge) | Subtitles and translation | Media to subtitles to translation with GUI/TUI/CLI modes. |
| [FunASR](https://github.com/modelscope/FunASR) | Speech recognition toolkit | Speech recognition toolkit with streaming and offline scenarios. |

### Image and Visual Workflows

| Project | Use case | Notes |
|---|---|---|
| [ComfyUI](https://github.com/comfyanonymous/ComfyUI) | Node-based image workflow | Local visual generation workflow with reusable graph pipelines. |
| [stable-diffusion-webui](https://github.com/AUTOMATIC1111/stable-diffusion-webui) | Image generation UI | Classic local Stable Diffusion web UI with a huge extension ecosystem. |

### Personal Knowledge and Notes

| Project | Use case | Notes |
|---|---|---|
| [Khoj](https://github.com/khoj-ai/khoj) | Personal AI second brain | Local-first personal knowledge assistant with search/chat flows. |
| [Screenpipe](https://github.com/screenpipe/screenpipe) | Screen and audio recall | Search locally captured screen text and audio history through MCP or a local API. Source-available under the Screenpipe Commercial License; configured cloud AI, transcription, sync and integrations can transmit context off-device. |
| [Obsidian Copilot](https://github.com/logancyang/obsidian-copilot) | Obsidian assistant | LLM assistant inside Obsidian notes. |
| [vibe-trading-bot](https://github.com/StaryMoon/vibe-trading-bot) | Trading research dashboard | Risk-first paper/sandbox/live-gated crypto assistant with Obsidian reports. |
| [DailyDesk](https://github.com/StaryMoon/DailyDesk) | Desktop planner | macOS glass desktop planner that can sit on the desktop like a local workflow widget. |
| [OpenHands](https://github.com/All-Hands-AI/OpenHands) | Software agent workspace | Agentic software-development workspace that can be connected to local providers. |

## Workstation Patterns

### Minimal private coding setup

```text
Ollama or llama.cpp
  -> Continue or aider
  -> local Git repo
  -> AICommit for commit messages
```

### Local research reading setup

```text
Ollama / LocalAI
  -> Open WebUI or AnythingLLM
  -> PDF / notes folder
  -> Obsidian / Khoj for recall
```

### Media note-taking setup

```text
whisper.cpp / ASR demo
  -> subtitles / transcript
  -> notes
  -> local summarization
```

## Selection Criteria

Projects are included when they are useful for a real local workstation:

- can run locally or self-hosted
- helps development, note-taking, speech, search, or desktop workflow
- has a clear README or setup path
- works with open model backends, local APIs, or private data workflows
- can be combined with at least one other tool in the workstation stack

## Add a Tool

Open a PR that updates `catalog.json` and the README. Please include:

- repository URL
- category
- primary use case
- short practical note

## License

CC0-1.0 for this list. Linked projects keep their own licenses.
