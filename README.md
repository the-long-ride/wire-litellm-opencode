# Wire LiteLLM and OpenCode/Codex together

A lightweight, web-based configuration generator wiring **LiteLLM Proxy**, **OpenCode**, and **Codex CLI** seamlessly together.

## Features

- **LiteLLM Multi-Provider Config**: Generate valid `config.yaml` files supporting multiple AI providers (OpenAI, Anthropic, Gemini, Azure, OpenRouter, Cloudflare Workers AI, Ollama, DeepSeek, etc.) with rate limits, timeouts, and fallback routing.
- **OpenCode Integration**: Export models and configurations tailored for OpenCode integration.
- **Codex CLI Integration**: 
  - Generate native Codex `config.toml` files.
  - Export customized `codex-model-catalog.json` with model capability metadata, reasoning effort tags, and probe statuses.
  - Generate setup and connection test PowerShell scripts (`Setup Codex PS1`, `Test Connection PS1`, probe tools).
- **Standalone Web App**: Built with vanilla HTML, CSS, and JavaScript. Runs directly in any modern browser without extra dependencies or build steps.

## Privacy & Security Guarantee

- **100% Client-Side Processing**: All key handling, configuration generation, and script exports execute purely within your browser. No data, API keys, or configurations are sent to any remote server or analytics service.
- **No Telemetry / No Backend**: There are no tracking scripts, backend servers, or third-party data collection APIs.
- **Ignored Local Secrets**: A [.gitignore](file:///.gitignore) is included to prevent generated `config.yaml`, `config.toml`, `.env`, keys, or test scripts from accidentally being committed to version control.

## Usage

Open `index.html` in your browser:

```bash
# Open index.html in default browser
start index.html   # On Windows
open index.html    # On macOS
xdg-open index.html # On Linux
```
