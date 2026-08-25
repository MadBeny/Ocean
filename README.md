<div align="center">

# Ocean

**A sleek desktop chat client for your local LLMs — powered by LM Studio.**

![Go](https://img.shields.io/badge/Go-00ADD8?style=for-the-badge&logo=go&logoColor=white)
![Wails](https://img.shields.io/badge/Wails-4F9EF7?style=for-the-badge)
![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black)
![CSS](https://img.shields.io/badge/CSS-555555?style=for-the-badge&logo=css3&logoColor=white)

</div>

---

## Requirements

Before you start, make sure you have the following set up:

### 1. Install LM Studio

Download and install [LM Studio](https://lmstudio.ai/download) — it runs your models locally on your system.

### 2. Enable the Local API Server in LM Studio

Open **Settings → Local Model API** and turn on these two options:

| Option | Why you need it |
| :--- | :--- |
| **Enable Local API Server** | Starts the OpenAI-compatible server at `http://localhost:1234/v1` that Ocean talks to. It only listens on your own computer — nothing is exposed to the internet. |
| **CORS (allow requests from any origin)** | Ocean runs in a desktop webview with its own app origin, so LM Studio must accept cross-origin requests from it. This still keeps everything local. |

> 💡 Don't worry about these toggles sounding "server-like" — the API never leaves your system. It's simply how Ocean and LM Studio talk to each other locally. No configuration is needed; `http://localhost:1234/v1` works out of the box.

### 3. Install Ocean

Download **OceanInstaller** from this repository and run it. That's it — no manual setup required.

### 4. Get a model

Pick whichever way is easier for you:

- **Easiest:** In LM Studio, open the **Explore** tab, find a model you like, and download it with one click.
- **Or bring your own GGUF:** Download any `.gguf` file from [Hugging Face](https://huggingface.co/models), then use the **Import Model** option in Ocean — it copies the file straight into LM Studio's local models folder, so no internet connection is needed at import time.

Once a model appears in LM Studio's list, select it in Ocean and start chatting.

Enjoy!
