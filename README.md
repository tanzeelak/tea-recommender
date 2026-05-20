# Sage: Your Tea-Savvy Friend

A voice AI agent that acts as an in-store tea guide for a specialty tea boutique. Sage knows her teas — aged whites, puerh cakes, GABA oolong, florals, global teas — and gives direct, prescriptive recommendations based on what you're dealing with, how you're feeling, or what vibe you're going for.

## What it does

- Opens with a featured tea recommendation
- Listens to what you need (symptom, mood, desire) and recommends a specific tea for it
- Covers health benefits, terroir, aging, and vibe-matching across a wide range of teas
- Speaks and listens — fully voice-driven conversation

## Tech stack

| Layer | What |
|---|---|
| Voice AI | [AssemblyAI Voice Agent API](https://www.assemblyai.com) — real-time STT, LLM, TTS over WebSocket |
| Audio capture | Web Audio API — `AudioWorklet` capturing mic as PCM16 at 24kHz |
| Audio playback | Web Audio API — streaming PCM16 chunks decoded and scheduled via `AudioContext` |
| Frontend | Vanilla HTML/CSS/JS, single file, no build step |

## Running it

Open `voice-agent.html` directly in a browser. No server needed.

The AssemblyAI API key is pre-configured. Click **Connect** to start talking to Sage.

## File structure

```
voice-agent.html   # Everything — UI, styles, audio pipeline, WebSocket client
README.md
```
