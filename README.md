<div align="center">

# 🌐 pi-zyloo-provider

**48 models across 9 families via [Zyloo](https://zyloo.io)**

_Claude, GPT, Gemini, Grok, Kimi, GLM, DeepSeek, Qwen & MiniMax — one OpenAI-compatible endpoint for [pi](https://github.com/earendil-works/pi-coding-agent)._

[![pi extension](https://img.shields.io/badge/pi-extension-blueviolet)](https://github.com/earendil-works/pi-coding-agent)
[![npm version](https://img.shields.io/npm/v/pi-zyloo-provider)](https://www.npmjs.com/package/pi-zyloo-provider)
[![license](https://img.shields.io/badge/license-MIT-blue)](./LICENSE)

</div>

---

## Features

- **One endpoint, every family** — Anthropic Claude, OpenAI GPT, Google Gemini, xAI Grok, Moonshot Kimi, Zhipu GLM, DeepSeek, Qwen & MiniMax behind a single OpenAI-compatible `/v1/chat/completions` API
- **Reasoning models** — thinking mode with `reasoning_effort` / `reasoning_content` on Claude, GPT, Gemini, GLM, DeepSeek, Qwen & MiniMax
- **Vision models** — image input on Claude, GPT, Gemini, Grok, Kimi & MiniMax M3
- **Tool use** — function calling support
- **Streaming** — real-time token streaming
- **Stale-While-Revalidate** — zero-latency startup from the embedded catalog, with a background refresh against `https://api.zyloo.io/v1/models`

> **Endpoint note:** `api.zyloo.ai` has no DNS A record. The live API is served at **`api.zyloo.io`**; `https://zyloo.ai/v1/*` 301-redirects to `https://api.zyloo.io/v1/*`.

## Available Models

| Model | Provider | Context | Vision | Reasoning | Input $/M | Output $/M |
|-------|---------|---------|--------|-----------|-----------|------------|
| Claude Fable 5 | Anthropic | 1.0M | ✅ | ✅ | $10.00 | $50.00 |
| Claude Opus 4.6 | Anthropic | 1.0M | ✅ | ✅ | $5.00 | $25.00 |
| Claude Opus 4.6 Thinking | Anthropic | 1.0M | ✅ | ✅ | $5.00 | $25.00 |
| Claude Opus 4.7 | Anthropic | 1.0M | ✅ | ✅ | $5.00 | $25.00 |
| Claude Opus 4.7 Thinking | Anthropic | 1.0M | ✅ | ✅ | $5.00 | $25.00 |
| Claude Opus 4.8 | Anthropic | 1.0M | ✅ | ✅ | $5.00 | $25.00 |
| Claude Opus 4.8 Thinking | Anthropic | 1.0M | ✅ | ✅ | $5.00 | $25.00 |
| Claude Opus 5 | Anthropic | 1.0M | ✅ | ✅ | $5.00 | $25.00 |
| Claude Opus 5 Thinking | Anthropic | 1.0M | ✅ | ✅ | $5.00 | $25.00 |
| Claude Sonnet 4.6 | Anthropic | 1.0M | ✅ | ✅ | $3.00 | $15.00 |
| Claude Sonnet 5 | Anthropic | 1.0M | ✅ | ✅ | $3.00 | $15.00 |
| DeepSeek V3.1 | DeepSeek | 164K | ❌ | ✅ | $0.27 | $0.95 |
| DeepSeek V3.2 | DeepSeek | 164K | ❌ | ✅ | $0.23 | $0.34 |
| DeepSeek V4 Flash | DeepSeek | 1.0M | ❌ | ✅ | $0.14 | $0.28 |
| DeepSeek V4 Pro | DeepSeek | 1.0M | ❌ | ✅ | $0.43 | $0.87 |
| Gemini 2.5 Flash | Google | 1.0M | ✅ | ✅ | $0.30 | $2.50 |
| Gemini 3 Flash Preview | Google | 1.0M | ✅ | ✅ | $0.50 | $3.00 |
| Gemini 3 Pro | Google | 1.0M | ✅ | ✅ | $2.00 | $12.00 |
| Gemini 3 Pro Preview | Google | 1.0M | ✅ | ✅ | $2.00 | $12.00 |
| Gemini 3.1 Flash Lite Preview | Google | 1.0M | ✅ | ✅ | $0.25 | $1.50 |
| Gemini 3.1 Pro Preview | Google | 1.0M | ✅ | ✅ | $2.00 | $12.00 |
| Gemini 3.5 Flash | Google | 1.0M | ✅ | ✅ | $1.50 | $9.00 |
| Gemini 3.6 Flash | Google | 1.0M | ✅ | ✅ | $1.50 | $9.00 |
| GLM-4.7 | Zhipu | 205K | ❌ | ✅ | **Free** | **Free** |
| GLM-5 | Zhipu | 200K | ❌ | ✅ | **Free** | **Free** |
| GLM-5.1 | Zhipu | 200K | ❌ | ✅ | **Free** | **Free** |
| GLM-5.2 | Zhipu | 1.0M | ❌ | ✅ | **Free** | **Free** |
| GPT-4.1 | OpenAI | 1.0M | ✅ | ❌ | $2.00 | $8.00 |
| GPT-4o | OpenAI | 128K | ✅ | ❌ | $2.50 | $10.00 |
| GPT-5.1 | OpenAI | 400K | ✅ | ✅ | $1.25 | $10.00 |
| GPT-5.2 | OpenAI | 400K | ✅ | ✅ | $1.75 | $14.00 |
| GPT-5.4 | OpenAI | 272K | ✅ | ✅ | $2.50 | $15.00 |
| GPT-5.5 | OpenAI | 272K | ✅ | ✅ | $5.00 | $30.00 |
| GPT-5.6 Luna | OpenAI | 272K | ✅ | ✅ | $5.00 | $30.00 |
| GPT-5.6 Sol | OpenAI | 272K | ✅ | ✅ | $5.00 | $30.00 |
| GPT-5.6 Terra | OpenAI | 272K | ✅ | ✅ | $5.00 | $30.00 |
| Grok 4.3 | xAI | 1.0M | ✅ | ✅ | $1.25 | $2.50 |
| Grok 4.5 | xAI | 1.0M | ✅ | ✅ | $1.25 | $2.50 |
| Grok Build 0.1 | xAI | 256K | ✅ | ✅ | $1.00 | $2.00 |
| Kimi K2 Thinking | Moonshot | 262K | ❌ | ✅ | $0.60 | $2.50 |
| Kimi K2.5 | Moonshot | 262K | ✅ | ✅ | $0.60 | $3.00 |
| Kimi K2.6 | Moonshot | 262K | ✅ | ✅ | $0.95 | $4.00 |
| Kimi K2.7 Code | Moonshot | 262K | ✅ | ✅ | $0.95 | $4.00 |
| Kimi K3 | Moonshot | 262K | ✅ | ✅ | $0.95 | $4.00 |
| MiniMax M2.5 | MiniMax | 205K | ❌ | ✅ | $0.15 | $0.90 |
| MiniMax M3 | MiniMax | 512K | ✅ | ✅ | $0.60 | $2.40 |
| Qwen3 Max | Qwen | 262K | ❌ | ❌ | $0.78 | $3.90 |
| Qwen3.7 Max | Qwen | 1.0M | ❌ | ✅ | $1.25 | $3.75 |

> **Pricing** reflects each model's native upstream provider (sourced from pi's built-in model catalog) where available. Zyloo's `/v1/models` endpoint exposes **no pricing**, and Zyloo may apply its own rates or markup — verify against your [Zyloo dashboard](https://zyloo.io/dashboard/billing). Models not yet present in any upstream catalog (e.g. GPT-5.6, Claude Opus 5, Gemini 3.6 Flash, Gemini 3 Pro, Grok 4.5, Kimi K3, GLM-5) use estimates from their closest known sibling.

## Installation

### Option 1: Using `pi install` (Recommended)

Install directly from GitHub:

```bash
pi install https://github.com/monotykamary/pi-zyloo-provider
```

Then set your API key and run pi:
```bash
# Recommended: add to auth.json
# See Authentication section below

# Or set as environment variable
export ZYLOO_API_KEY=your-api-key-here

pi
```

Get your API key from [zyloo.io](https://zyloo.io).

### Option 2: Manual Clone

1. Clone this repository:
   ```bash
   git clone https://github.com/monotykamary/pi-zyloo-provider.git
   cd pi-zyloo-provider
   ```

2. Set your Zyloo API key:
   ```bash
   # Recommended: add to auth.json
   # See Authentication section below

   # Or set as environment variable
   export ZYLOO_API_KEY=your-api-key-here
   ```

3. Run pi with the extension:
   ```bash
   pi -e /path/to/pi-zyloo-provider
   ```

### Option 3: Via npm

Install the package from npm:
```bash
npm install pi-zyloo-provider
# or
pnpm add pi-zyloo-provider
```

Then load it by path (npm installs into `node_modules`):
```bash
pi -e ./node_modules/pi-zyloo-provider
```

## Authentication

The Zyloo API key can be configured in multiple ways (resolved in this order):

1. **`auth.json`** (recommended) — Add to `~/.pi/agent/auth.json`:
   ```json
   { "zyloo": { "type": "api_key", "key": "your-api-key" } }
   ```
   The `key` field supports literal values, env var names, and shell commands (prefix with `!`). See [pi's auth file docs](https://github.com/badlogic/pi-mono) for details.
2. **Runtime override** — Use the `--api-key` CLI flag
3. **Environment variable** — Set `ZYLOO_API_KEY`

Get your API key from [zyloo.io](https://zyloo.io).

## Environment Variables

| Variable | Required | Description |
|----------|----------|-------------|
| `ZYLOO_API_KEY` | No | Your Zyloo API key (fallback if not in auth.json) |

## Configuration

Add to your pi configuration for automatic loading:

```json
{
  "extensions": [
    "/path/to/pi-zyloo-provider"
  ]
}
```

## Usage

Once loaded, select a model with:

```
/model zyloo zyloo/claude-opus-4-8
```

Or use `/models` to browse all available Zyloo models.

### Reasoning Effort

For reasoning models, control thinking depth:

```
/reasoning high
```
Values: `none`, `low`, `medium`, `high` (and `xhigh`/`max` where the model exposes it via `thinkingLevelMap`).

## API Compatibility

Zyloo provides an OpenAI-compatible Chat Completions proxy. Reasoning format and role handling are configured per model family in `patch.json`:

| Family | Models | `thinkingFormat` | Reasoning Effort | Developer Role |
|--------|-------|-------------------|------------------|---------------|
| Anthropic Claude | `claude-*` | `openai` | ✅ | ✅ |
| OpenAI GPT (reasoning) | `gpt-5.*` | `openai` | ✅ | ✅ |
| OpenAI GPT (chat) | `gpt-4.1`, `gpt-4o` | — | — | ✅ |
| Google Gemini | `gemini-*` | `openai` | ✅ | ✅ |
| xAI Grok | `grok-*` | — (inherent) | ❌ | ❌ (`system`) |
| Moonshot Kimi | `kimi-*` | `deepseek` | ❌ | ❌ (`system`) |
| Zhipu GLM | `glm-5.2` | `openai` | ✅ | ❌ (`system`) |
| Zhipu GLM | `glm-4.7`, `glm-5`, `glm-5.1` | `openai` | ❌ | ❌ (`system`) |
| DeepSeek | `deepseek-*` | `deepseek` | ✅ (`high`/`max`) | ❌ (`system`) |
| Qwen | `qwen3.7-max` | `openai` | ✅ | ✅ |
| Qwen | `qwen3-max` (chat) | — | — | ✅ |
| MiniMax | `minimax-*` | `openai` | ✅ | ✅ |

Key notes:

| Aspect | Behavior |
|--------|----------|
| API | `openai-completions` (Chat Completions) |
| Base URL | `https://api.zyloo.io/v1` |
| Max tokens field | Both `max_tokens` and `max_completion_tokens` accepted |
| Reasoning output | `reasoning_content` in responses |
| `store` parameter | Not sent (`supportsStore: false`) |

> The Zyloo `/v1/models` endpoint only returns model IDs and `owned_by` — no pricing, context lengths, or reasoning flags. `patch.json` provides these based on each upstream provider's published specifications.

## Updating Models

Run the update script to fetch the latest models from Zyloo's API:

```bash
export ZYLOO_API_KEY=your-api-key
node scripts/update-models.js
```

This will:
1. Fetch models from `https://api.zyloo.io/v1/models`
2. Preserve pricing and compat from existing `models.json`
3. Apply overrides from `patch.json`
4. Update `models.json` and the README model table

A GitHub Actions workflow can run this daily and open a PR if models have changed.

## License

MIT
