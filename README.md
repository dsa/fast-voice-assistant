# Insanely fast AI voice assistant in 50 LOC

This repo contains everything you need to run your own real-time voice assistant that responds to you in less than 500ms.

It uses:
🌐 [LiveKit](https://github.com/livekit) transport
👂 [Deepgram](https://deepgram.com/) STT
🧠 [Cerebras](https://inference.cerebras.ai/) LLM
🗣️ [Cartesia](https://cartesia.ai/) TTS

To get this running, first clone the repo.

## Run the agent

1. `python -m venv .venv`
2. `source .venv/bin/activate`
3. `pip install -r requirements.txt`
4. `cp .env.example .env`
5. add values for keys in `.env`
6. `python main.py dev`

## Run a client

1. Go to the [playground](https://agents-playground.livekit.io/#cam=0&mic=1&video=0&audio=1&chat=0&theme_color=amber)
2. Choose the same LiveKit Cloud project you used in the agent's `.env` and click `Connect`

Note: playground code is [here](https://github.com/livekit/agents-playground) if you want to customize/build your own.
