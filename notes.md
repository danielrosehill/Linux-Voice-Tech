# Notes & Background

## What's Here

This repository gathers voice technology tools that are accessible to Linux desktop users. The collection spans a wide range:

- **Real-time transcription** ("voice typing") - tools for live dictation
- **Asynchronous transcription** - note-taking apps, meeting transcribers, audio-to-text converters
- **Voice assistants** - voice-controlled interfaces and assistants
- **Text-to-speech** - TTS tools and frameworks
- **Development frameworks** - libraries and toolkits for building voice applications

For a tool to be "Linux accessible," it needs to offer one of: a native GUI, a CLI, a web UI (self-hosted or cloud), or SaaS with browser access.

## The Voice Tech Boom on Linux

For years, voice support on Linux was sparse. Major dictation providers ignored the platform due to small desktop market share, and voice assistant projects struggled without reliable transcription backends.

Since OpenAI open-sourced Whisper, the landscape has transformed dramatically. We've gone from a handful of options to an explosion of projects — now presenting a familiar Linux challenge: many splintered efforts across the ecosystem.

I created this repo as a Linux user passionate about voice technology, wanting to gather and organize the rapidly growing list of tools. What was once a short list is now quite extensive, and my aim is to help others (and myself) navigate and explore this space.

## AI / Human Division Of Labor

Me: raw notes, resource location, categorisation.
Claude: updating readme, polishing language.

## Foundations of Transcription: Models + Wrappers

The foundation of modern voice technology is ASR (automatic speech recognition) models.

Typically these are chained with other smaller models to:

- Add punctuation
- Add voice activity detection (some tools)
- Add speaker identification/diarisation (some tools)

ASR is inherently a-lingual. However, models are fine-trained on datasets of language-specific models. Major world languages are widely available while others are works in progress.

Because Whisper is open source, you'll encounter more than one type of Whisper:

- Whisper variants (Faster Whisper, Crisper Whisper, etc)
- The original Whisper (as maintained by OpenAI)
- Various wrappers that intend to bridge between local inference and other languages

Some of what you'll find on a Github Whisper crawl is ready-to-use tooling (e.g. GUIs/CLIs that do the bundling).

In other cases, it's components that you assemble yourself: model + component + frontend (or CLI) = useable solution.

Hotkey support is also very common: I use a simple $5 USB button from Aliexpress (one of my greatest Ali buys!). But you can use a keyboard shortcut. Either way, after a few minutes of voice typing, the need is quickly apparent.

## GPU Acceleration

For STT/voice typing, you'll find that GPU acceleration is often limited to NVIDIA/CUDA. Having an NVIDIA GPU makes life easier when running local models!

## Wayland Compatibility

Wayland presents challenges with virtual keyboards.

[ydotool](https://github.com/ReimuNotMoe/ydotool) (and its daemon) are commonly used to attempt to provide virtual keyboard support while other implementations implement at the kernel level.

## STT Deployment Patterns

Projects typically support either **local STT** or **cloud STT**, and less commonly both:

- **Local-only STT**: These implementations usually assume or install a local copy of Whisper or other models, offering complete privacy and offline functionality
- **Cloud-only STT**: Apps that rely exclusively on cloud inference, either supporting a single provider or offering multiple provider choices
- **Hybrid approaches**: Some projects enable users to choose between local or commercial/cloud-hosted STT

Among cloud STT integrations, **Whisper** (via OpenAI or other providers) remains the most common integration. However, a small but growing selection of projects are emerging that use **Deepgram** for cloud-based STT.

## How This Repository Is Organized

Given the large number of projects, I've attempted to categorize them along several dimensions:

- **Wayland support**: Projects explicitly supporting Wayland virtual input (important for modern Linux desktop users)
- **Hardware focus**: CPU-centric vs. GPU-optimized implementations
- **Transcription mode**: Real-time (streaming) vs. asynchronous (batch/upload)

Beyond these technical distinctions, projects roughly fall into three functional categories:

1. **Pure ASR tools**: CLIs, desktop GUIs, or web UIs focused solely on transcription — either real-time or asynchronous (upload and transcribe).

2. **ASR + rewrite**: Tools that combine speech recognition with LLM post-processing. The raw transcript gets refined through a language model to fix errors, improve formatting, or restructure into specific formats (emails, notes, etc.).

3. **ASR + action**: Tools that transcribe speech and then translate the result into actions — voice-to-code, voice-to-MCP, voice commands, computer use agents, etc.

## Inclusion Criteria

This repository focuses on modern ASR projects from the current AI-accelerated era, excluding pre-Whisper legacy STT tools. For detailed scope information, see our [Inclusion Criteria](inclusion-criteria.md) page.

| Scope | Category | Description |
|-------|----------|-------------|
| ✅ In Scope | STT | Speech-to-text tools and applications |
| ✅ In Scope | Voice Assistants | Voice-controlled assistant applications |
| ✅ In Scope | Voice-to-X | Voice-to-MCP, voice-to-commands, and similar tools |
| ✅ In Scope | TTS | Text-to-speech synthesis tools |
