# Local AI Workstation Stacks

This page collects practical stacks rather than individual tools. The goal is to reduce choice paralysis.

## Stack 1: Private Coding Assistant

Use this when you want code help without sending every file to a hosted model.

```text
Ollama / llama.cpp
  -> Continue or aider
  -> local Git repo
  -> AICommit for commit messages
```

Good for:

- private project notes
- small refactors
- local coding practice
- offline commit message drafts

Watch out:

- smaller local models may struggle with large repo-wide edits
- always review generated diffs
- keep secrets out of prompts and logs

## Stack 2: Research Reading Workbench

Use this when your main objects are papers, notes, and PDFs.

```text
Ollama / LocalAI
  -> Open WebUI / AnythingLLM / Khoj
  -> PDF folder
  -> Obsidian notes
```

Good for:

- daily paper reading
- literature maps
- project memory
- local RAG over notes

Watch out:

- OCR quality matters more than the chat UI
- chunking and citation display decide whether the workflow is trustworthy
- keep a manual note trail for anything used in a paper

## Stack 3: Audio and Meeting Notes

Use this when the raw material is lectures, meetings, or videos.

```text
whisper.cpp / FunASR
  -> transcript
  -> local summarization
  -> Obsidian or Markdown archive
```

Good for:

- lectures
- technical talks
- recorded meetings
- subtitle cleanup

Watch out:

- diarization is a separate problem
- code-switching can reduce ASR quality
- verify names, numbers, and citations manually

## Stack 4: Visual Ideation

Use this when you need local image-generation or visual workflow control.

```text
ComfyUI / stable-diffusion-webui
  -> local model folder
  -> reusable workflow graph
  -> exported assets
```

Good for:

- mockups
- icons
- illustration drafts
- controlled image pipelines

Watch out:

- model licenses vary
- image outputs may need attribution or filtering
- keep workflows versioned if you need reproducibility

## Stack 5: Personal Dashboard

Use this when you want local AI output to become a habit instead of a one-off chat.

```text
local model/runtime
  -> small dashboard or desktop widget
  -> Markdown/SQLite state
  -> review loop
```

Examples:

- DailyDesk for desktop reminders and local workflow presence
- vibe-trading-bot for paper/sandbox trading reports
- custom Obsidian dashboards for daily research briefings

The durable pattern is simple: model output should land in a file, a dashboard, or a review queue. If it only appears in a chat box, it is easy to lose.
