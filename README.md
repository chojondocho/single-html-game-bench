# Single HTML Game Bench

A zero-shot benchmark project comparing how different AI clients/models perform when asked to generate a complete game in **one single HTML file**.

This repository contains first-pass outputs (one shot, no iterative refinement) from multiple model/client combinations using the exact same prompt.

## Prompt Used

```text
Create a complete 3D horror game in a single HTML file, incorporating RPG and roguelike elements. The quality must be high enough to win a Game of the Year award. Do not stop until you determine that it can definitely win. Every element must be production-ready for release within that single HTML file alone.
```

## Live Play (GitHub Pages)

Base URL:

- https://chojondocho.github.io/single-html-game-bench/

## Personal Ranking (Subjective Result)

As of **February 17, 2026**, based on direct hands-on play testing:

| Rank | Client + Model                  | Play                                                                                         |
| ---- | ------------------------------- | -------------------------------------------------------------------------------------------- |
| 1    | Claude Code - Opus 4.6          | [Play](https://chojondocho.github.io/single-html-game-bench/claudecode-opus-4-6.html)        |
| 2    | ChatGPT - GPT-5.2 Pro           | [Play](https://chojondocho.github.io/single-html-game-bench/chatgpt-gpt-5-2-pro.html)        |
| 3    | Claude Code - Sonnet 4.6        | [Play](https://chojondocho.github.io/single-html-game-bench/claudecode-sonnet-4-6.html)       |
| 4    | Gemini Web - Gemini 3.1 Pro Deepthink | [Play](https://chojondocho.github.io/single-html-game-bench/geminiweb-gemini-3-1-pro-deepthink.html)  |
| 5    | Codex - GPT-5.3 Codex High      | [Play](https://chojondocho.github.io/single-html-game-bench/codex-gpt-5-3-codex-high.html)   |
| 6    | Antigravity - Opus 4.6          | [Play](https://chojondocho.github.io/single-html-game-bench/antigravity-opus-4-6.html)       |
| 7    | Antigravity - Gemini 3 Pro      | [Play](https://chojondocho.github.io/single-html-game-bench/antigravity-gemini-3-pro.html)   |
| 8    | Codex - GPT-5.3 Codex XHigh     | [Play](https://chojondocho.github.io/single-html-game-bench/codex-gpt-5-3-codex-xhigh.html)  |
| 9    | Antigravity - Gemini 3 Flash    | [Play](https://chojondocho.github.io/single-html-game-bench/antigravity-gemini-3-flash.html) |
| 10   | Grok Web - Grok 4.20 (4 Agents) | [Play](https://chojondocho.github.io/single-html-game-bench/grokweb-grok-4-20-4agents.html)  |

## All Playable Builds (Direct Links)

- [claudecode-opus-4-6](https://chojondocho.github.io/single-html-game-bench/claudecode-opus-4-6.html)
- [chatgpt-gpt-5-2-pro](https://chojondocho.github.io/single-html-game-bench/chatgpt-gpt-5-2-pro.html)
- [claudecode-sonnet-4-6](https://chojondocho.github.io/single-html-game-bench/claudecode-sonnet-4-6.html)
- [codex-gpt-5-3-codex-high](https://chojondocho.github.io/single-html-game-bench/codex-gpt-5-3-codex-high.html)
- [antigravity-opus-4-6](https://chojondocho.github.io/single-html-game-bench/antigravity-opus-4-6.html)
- [antigravity-gemini-3-pro](https://chojondocho.github.io/single-html-game-bench/antigravity-gemini-3-pro.html)
- [codex-gpt-5-3-codex-xhigh](https://chojondocho.github.io/single-html-game-bench/codex-gpt-5-3-codex-xhigh.html)
- [antigravity-gemini-3-flash](https://chojondocho.github.io/single-html-game-bench/antigravity-gemini-3-flash.html)
- [grokweb-grok-4-20-4agents](https://chojondocho.github.io/single-html-game-bench/grokweb-grok-4-20-4agents.html)
- [geminiweb-gemini-3-1-pro-deepthink](https://chojondocho.github.io/single-html-game-bench/geminiweb-gemini-3-1-pro-deepthink.html)

## Benchmark Rules

- Single fixed prompt for all entries
- Zero-shot, one-pass generation only
- Output must be a single standalone HTML file
- No manual gameplay/system-level tuning after generation

## What This Benchmark Is (and Is Not)

- This is a personal, practical benchmark focused on raw first-pass capability.
- The ranking above is personal and subjective, based on the author's own play experience.
- It is not a formal scientific evaluation and does not claim universal ranking validity.
- Results can vary by date, model revision, system prompt, and runtime environment.

## Run Locally

If you want to run any build locally, you can open the file directly in your browser or serve this directory:

```bash
cd single-html-game-bench
python3 -m http.server 8080
```

Then open:

- http://localhost:8080/

## Why This Exists

The goal is simple: make generated game artifacts publicly playable and easy to compare, so anyone can judge quality hands-on rather than by screenshots or claims.

## License and Disclaimer

- Licensed under the [MIT License](./LICENSE).
- This repository contains AI-generated benchmark outputs and is provided **as is**, without warranty of any kind.
