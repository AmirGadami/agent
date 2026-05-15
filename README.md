# Amir Agent — AI Career Assistant

An AI-powered personal assistant that talks on my behalf — if you want to know anything about me, just ask it.

🔗 **Live demo:** https://huggingface.co/spaces/amirghadami/Amir_Agent_Resume

## What you can ask it

- Who is Amir and what does he do?
- What is his research background and publications?
- What projects has he built?
- What are his technical skills?
- Is he open to new opportunities?
- How can I get in touch with him?

The agent will answer as if you're speaking directly with me — professionally and accurately, based on my actual resume and background.

## How it works

The agent is powered by **GPT-4o-mini** and grounded in my real resume and personal summary, injected into the system prompt. It has two tools:

- `record_user_details` — if you'd like to connect, share your email and it will notify me instantly
- `record_unknown_question` — any question it can't answer gets flagged so I can improve it

I get a **real-time push notification** via Pushover whenever someone engages or leaves their contact details.

## Tech stack

- [OpenAI](https://openai.com) — GPT-4o-mini for conversation
- [Gradio](https://gradio.app) — chat interface
- [pypdf](https://pypdf.readthedocs.io) — PDF parsing
- [Pushover](https://pushover.net) — push notifications

## Environment variables

| Variable | Description |
|---|---|
| `OPENAI_API_KEY` | Your OpenAI API key |
| `PUSHOVER_USER` | Your Pushover user key |
| `PUSHOVER_TOKEN` | Your Pushover app token |