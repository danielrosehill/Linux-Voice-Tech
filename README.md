# Linux Voice Tech

![alt text](banner.png)

## An index of voice technology tools accessible to Linux users

![Last Updated](https://img.shields.io/badge/Last%20Updated-March%2029%2C%202026-blue?style=flat-square)
![Repository Type](https://img.shields.io/badge/Type-Index-green?style=flat-square)
![Resources](https://img.shields.io/badge/Resources-120%2B-orange?style=flat-square)
![License](https://img.shields.io/badge/License-MIT-yellow?style=flat-square)

Star counts and last commit dates are shown via shields.io badges and update dynamically.

For background, notes on how the repo is organized, and inclusion criteria, see [notes.md](notes.md). For a getting started guide, see [starting-points.md](starting-points.md).

## Keywords

- Automatic speech recognition (ASR)
- Speech-to-text (STT)
- Text-to-speech (TTS)
- Linux voice typing
- Linux dictation
- Linux TTS
- Voice control
- Transcription

## Quick Navigation

| Section | What's in it |
|---------|-------------|
| [Wayland-Compatible STT](#stt-tools-with-wayland-support) | Tools with explicit Wayland virtual input support |
| [Voice Typing — GUIs](#voice-typing--guis) | Desktop apps for dictation and transcription |
| [Voice Typing — CLIs](#voice-typing--clis) | Command-line dictation and transcription tools |
| [Voice Notes & AI-Enhanced](#voice-notes--ai-enhanced-transcription) | Note-taking with AI post-processing |
| [Real-Time Streaming STT](#real-time-streaming-stt) | Low-latency, live transcription libraries |
| [Self-Hosted / Web UI](#self-hosted--web-ui) | Docker/web-based transcription services |
| [Cloud STT / API-Based](#cloud-stt--api-based-tools) | Tools using OpenAI, Deepgram, or other cloud APIs |
| [Voice Assistants](#voice-assistants) | Voice-controlled assistant applications |
| [Voice Commands & Automation](#voice-commands--automation) | Voice-to-action, voice-to-MCP, computer control |
| [Toolkits & Frameworks](#toolkits--frameworks) | Developer libraries for building voice apps |
| [Whisper Variants & Optimizations](#whisper-variants--optimizations) | Faster/smaller/better Whisper implementations |
| [Complementary Tools](#complementary-tools) | VAD, diarization, noise suppression |
| [Text-to-Speech (TTS)](#text-to-speech-tts) | TTS tools and frameworks |
| [MCP Servers](#mcp-servers) | Model Context Protocol voice servers |
| [Awesome Lists](#awesome-lists) | Other curated voice tech lists |
| [Community Resources](#community-resources) | GitHub topics, subreddits |

---

## STT Tools with Wayland Support

Projects with explicit Wayland support. Particularly valuable for users on modern Linux desktops (GNOME, KDE Plasma on Wayland, Hyprland, Sway, niri, etc.) where X11 virtual input methods don't work.

| Repository | Stars | Last Updated | Description |
|------------|-------|--------------|-------------|
| [**dictation-tools**](https://github.com/gfreeau/dictation-tools) | ![Stars](https://img.shields.io/github/stars/gfreeau/dictation-tools?style=flat-square) | ![Last Commit](https://img.shields.io/github/last-commit/gfreeau/dictation-tools?style=flat-square) | Dictation tools with Wayland support |
| [**freespeak**](https://github.com/Zetaphor/freespeak) | ![Stars](https://img.shields.io/github/stars/Zetaphor/freespeak?style=flat-square) | ![Last Commit](https://img.shields.io/github/last-commit/Zetaphor/freespeak?style=flat-square) | Voice dictation with Wayland support |
| [**hyprvoice**](https://github.com/LeonardoTrapani/hyprvoice) | ![Stars](https://img.shields.io/github/stars/LeonardoTrapani/hyprvoice?style=flat-square) | ![Last Commit](https://img.shields.io/github/last-commit/LeonardoTrapani/hyprvoice?style=flat-square) | Voice dictation for Hyprland |
| [**hyprwhspr**](https://github.com/goodroot/hyprwhspr) | ![Stars](https://img.shields.io/github/stars/goodroot/hyprwhspr?style=flat-square) | ![Last Commit](https://img.shields.io/github/last-commit/goodroot/hyprwhspr?style=flat-square) | Whisper-based voice input for Hyprland |
| [**local-dictation-assistant**](https://github.com/Wiecek-K/local-dictation-assistant) | ![Stars](https://img.shields.io/github/stars/Wiecek-K/local-dictation-assistant?style=flat-square) | ![Last Commit](https://img.shields.io/github/last-commit/Wiecek-K/local-dictation-assistant?style=flat-square) | Local dictation assistant with Wayland support |
| [**niri-transcribe**](https://github.com/sevos/niri-transcribe) | ![Stars](https://img.shields.io/github/stars/sevos/niri-transcribe?style=flat-square) | ![Last Commit](https://img.shields.io/github/last-commit/sevos/niri-transcribe?style=flat-square) | Transcription tool for niri compositor |
| [**swictation**](https://github.com/robertelee78/swictation) | ![Stars](https://img.shields.io/github/stars/robertelee78/swictation?style=flat-square) | ![Last Commit](https://img.shields.io/github/last-commit/robertelee78/swictation?style=flat-square) | Voice dictation for Sway/Wayland |
| [**TalkType (ronb1964)**](https://github.com/ronb1964/TalkType) | ![Stars](https://img.shields.io/github/stars/ronb1964/TalkType?style=flat-square) | ![Last Commit](https://img.shields.io/github/last-commit/ronb1964/TalkType?style=flat-square) | Privacy-first voice dictation for Linux Wayland. Press key to talk, release to type. Whisper AI, 100% offline |
| [**vocalinux**](https://github.com/jatinkrmalik/vocalinux) | ![Stars](https://img.shields.io/github/stars/jatinkrmalik/vocalinux?style=flat-square) | ![Last Commit](https://img.shields.io/github/last-commit/jatinkrmalik/vocalinux?style=flat-square) | Offline voice dictation for Linux. Whisper.cpp, Whisper & VOSK engines, GPU-accelerated, X11 + Wayland |
| [**voice-typing-linux**](https://github.com/GitJuhb/voice-typing-linux) | ![Stars](https://img.shields.io/github/stars/GitJuhb/voice-typing-linux?style=flat-square) | ![Last Commit](https://img.shields.io/github/last-commit/GitJuhb/voice-typing-linux?style=flat-square) | Voice typing for Linux with Wayland support |
| [**wayland-voice-dictation**](https://github.com/MasonRhodesDev/wayland-voice-dictation) | ![Stars](https://img.shields.io/github/stars/MasonRhodesDev/wayland-voice-dictation?style=flat-square) | ![Last Commit](https://img.shields.io/github/last-commit/MasonRhodesDev/wayland-voice-dictation?style=flat-square) | Voice dictation designed for Wayland |
| [**whisper-wayland**](https://github.com/Andrewske/whisper-wayland) | ![Stars](https://img.shields.io/github/stars/Andrewske/whisper-wayland?style=flat-square) | ![Last Commit](https://img.shields.io/github/last-commit/Andrewske/whisper-wayland?style=flat-square) | Whisper integration for Wayland |
| [**whispy**](https://github.com/daaku/whispy) | ![Stars](https://img.shields.io/github/stars/daaku/whispy?style=flat-square) | ![Last Commit](https://img.shields.io/github/last-commit/daaku/whispy?style=flat-square) | STT tool with Wayland support |

---

## Voice Typing — GUIs

Desktop applications for dictation and transcription with graphical interfaces.

| Repository | Stars | Last Updated | Description |
|------------|-------|--------------|-------------|
| [**AI-Typer-V2**](https://github.com/danielrosehill/AI-Typer-V2) | ![Stars](https://img.shields.io/github/stars/danielrosehill/AI-Typer-V2?style=flat-square) | ![Last Commit](https://img.shields.io/github/last-commit/danielrosehill/AI-Typer-V2?style=flat-square) | Voice dictation with multimodal AI cleanup — speak naturally, get polished text |
| [**aTrain**](https://github.com/JuergenFleiss/aTrain) | ![Stars](https://img.shields.io/github/stars/JuergenFleiss/aTrain?style=flat-square) | ![Last Commit](https://img.shields.io/github/last-commit/JuergenFleiss/aTrain?style=flat-square) | Audio transcription training tool |
| [**audiov**](https://github.com/WhiteSmoogy/audiov) | ![Stars](https://img.shields.io/github/stars/WhiteSmoogy/audiov?style=flat-square) | ![Last Commit](https://img.shields.io/github/last-commit/WhiteSmoogy/audiov?style=flat-square) | Speech-to-text, voice-typing, dictation software for Linux distributions |
| [**Buzz**](https://github.com/chidiwilliams/buzz) | ![Stars](https://img.shields.io/github/stars/chidiwilliams/buzz?style=flat-square) | ![Last Commit](https://img.shields.io/github/last-commit/chidiwilliams/buzz?style=flat-square) | Offline audio transcription and translation. Supports Whisper, Whisper.cpp, Faster-Whisper. Available via Flatpak/Snap. Vulkan GPU support |
| [**dsnote**](https://github.com/mkiol/dsnote) | ![Stars](https://img.shields.io/github/stars/mkiol/dsnote?style=flat-square) | ![Last Commit](https://img.shields.io/github/last-commit/mkiol/dsnote?style=flat-square) | Speech Note Linux app. Note taking, reading and translating with offline Speech to Text, Text to Speech and Machine translation |
| [**LinuxWhisper**](https://github.com/vitali87/LinuxWhisper) | ![Stars](https://img.shields.io/github/stars/vitali87/LinuxWhisper?style=flat-square) | ![Last Commit](https://img.shields.io/github/last-commit/vitali87/LinuxWhisper?style=flat-square) | Whisper for Linux |
| [**maVoice-Linux**](https://github.com/lliWcWill/maVoice-Linux) | ![Stars](https://img.shields.io/github/stars/lliWcWill/maVoice-Linux?style=flat-square) | ![Last Commit](https://img.shields.io/github/last-commit/lliWcWill/maVoice-Linux?style=flat-square) | Voice control for Linux |
| [**mint-whisper**](https://github.com/codankra/mint-whisper) | ![Stars](https://img.shields.io/github/stars/codankra/mint-whisper?style=flat-square) | ![Last Commit](https://img.shields.io/github/last-commit/codankra/mint-whisper?style=flat-square) | Whisper for Linux Mint |
| [**murmure**](https://github.com/Kieirra/murmure) | ![Stars](https://img.shields.io/github/stars/Kieirra/murmure?style=flat-square) | ![Last Commit](https://img.shields.io/github/last-commit/Kieirra/murmure?style=flat-square) | Fully local, private, cross-platform STT with LLM post-processing |
| [**OpenFlow**](https://github.com/logabell/OpenFlow) | ![Stars](https://img.shields.io/github/stars/logabell/OpenFlow?style=flat-square) | ![Last Commit](https://img.shields.io/github/last-commit/logabell/OpenFlow?style=flat-square) | Local speech-to-text app for Linux |
| [**OpenTypeless**](https://github.com/tover0314-w/opentypeless) | ![Stars](https://img.shields.io/github/stars/tover0314-w/opentypeless?style=flat-square) | ![Last Commit](https://img.shields.io/github/last-commit/tover0314-w/opentypeless?style=flat-square) | Cross-platform voice typing for Linux, macOS, and Windows with configurable STT providers and optional AI text polishing |
| [**OpenWispr**](https://github.com/imsidharthj/OpenWispr) | ![Stars](https://img.shields.io/github/stars/imsidharthj/OpenWispr?style=flat-square) | ![Last Commit](https://img.shields.io/github/last-commit/imsidharthj/OpenWispr?style=flat-square) | Open source Whisper-based voice assistant |
| [**Parakeet-Type-Ubuntu**](https://github.com/danielrosehill/Parakeet-Type-Ubuntu) | ![Stars](https://img.shields.io/github/stars/danielrosehill/Parakeet-Type-Ubuntu?style=flat-square) | ![Last Commit](https://img.shields.io/github/last-commit/danielrosehill/Parakeet-Type-Ubuntu?style=flat-square) | On-device voice typing for Linux using Parakeet and NeMo ASR models via sherpa-onnx. No cloud, no GPU required |
| [**sotto**](https://github.com/Maciejonos/sotto) | ![Stars](https://img.shields.io/github/stars/Maciejonos/sotto?style=flat-square) | ![Last Commit](https://img.shields.io/github/last-commit/Maciejonos/sotto?style=flat-square) | Local speech-to-text transcription app for Linux using Whisper models |
| [**soundvibes**](https://github.com/kejne/soundvibes) | ![Stars](https://img.shields.io/github/stars/kejne/soundvibes?style=flat-square) | ![Last Commit](https://img.shields.io/github/last-commit/kejne/soundvibes?style=flat-square) | Speech-to-text for Linux that just works |
| [**TalkType (zyk42)**](https://github.com/zyk42/TalkType) | ![Stars](https://img.shields.io/github/stars/zyk42/TalkType?style=flat-square) | ![Last Commit](https://img.shields.io/github/last-commit/zyk42/TalkType?style=flat-square) | Cross-platform Electron voice writing assistant. ASR + LLM for understanding, polishing, and Q&A |
| [**TranscriptionSuite**](https://github.com/homelab-00/TranscriptionSuite) | ![Stars](https://img.shields.io/github/stars/homelab-00/TranscriptionSuite?style=flat-square) | ![Last Commit](https://img.shields.io/github/last-commit/homelab-00/TranscriptionSuite?style=flat-square) | Fully local, private STT app with speaker diarization, Audio Notebook mode, LM Studio integration, longform and live transcription |
| [**VoiceType**](https://github.com/danielrosehill/VoiceType) | ![Stars](https://img.shields.io/github/stars/danielrosehill/VoiceType?style=flat-square) | ![Last Commit](https://img.shields.io/github/last-commit/danielrosehill/VoiceType?style=flat-square) | Fork of Deepgram's Linux starter. CLI to GUI + hotkey support, API key editing, cost tracking |
| [**WhisperNow**](https://github.com/shinglyu/WhisperNow) | ![Stars](https://img.shields.io/github/stars/shinglyu/WhisperNow?style=flat-square) | ![Last Commit](https://img.shields.io/github/last-commit/shinglyu/WhisperNow?style=flat-square) | Real-time Whisper transcription |
| [**whisper-to-input-desktop**](https://github.com/Rosbifbr/whisper-to-input-desktop) | ![Stars](https://img.shields.io/github/stars/Rosbifbr/whisper-to-input-desktop?style=flat-square) | ![Last Commit](https://img.shields.io/github/last-commit/Rosbifbr/whisper-to-input-desktop?style=flat-square) | Desktop app using OpenAI's Whisper to transcribe audio and input it as text |
| [**whisper-ui**](https://github.com/schnoddelbotz/whisper-ui) | ![Stars](https://img.shields.io/github/stars/schnoddelbotz/whisper-ui?style=flat-square) | ![Last Commit](https://img.shields.io/github/last-commit/schnoddelbotz/whisper-ui?style=flat-square) | Whisper UI interface |
| [**whisperer**](https://github.com/mike-cr/whisperer) | ![Stars](https://img.shields.io/github/stars/mike-cr/whisperer?style=flat-square) | ![Last Commit](https://img.shields.io/github/last-commit/mike-cr/whisperer?style=flat-square) | Whisper-based transcription tool |
| [**whisply**](https://github.com/tsmdt/whisply) | ![Stars](https://img.shields.io/github/stars/tsmdt/whisply?style=flat-square) | ![Last Commit](https://img.shields.io/github/last-commit/tsmdt/whisply?style=flat-square) | A simple GUI for OpenAI Whisper |
| [**wisper**](https://github.com/taraksh01/wisper) | ![Stars](https://img.shields.io/github/stars/taraksh01/wisper?style=flat-square) | ![Last Commit](https://img.shields.io/github/last-commit/taraksh01/wisper?style=flat-square) | Voice dictation app for Linux. Type directly at cursor with AI-powered transcription |
| [**wispr-lite**](https://github.com/dosment/wispr-lite) | ![Stars](https://img.shields.io/github/stars/dosment/wispr-lite?style=flat-square) | ![Last Commit](https://img.shields.io/github/last-commit/dosment/wispr-lite?style=flat-square) | Lightweight Whisper-based transcription tool |

---

## Voice Typing — CLIs

Command-line dictation and transcription tools.

| Repository | Stars | Last Updated | Description |
|------------|-------|--------------|-------------|
| [**BlahST**](https://github.com/QuantiusBenignus/BlahST) | ![Stars](https://img.shields.io/github/stars/QuantiusBenignus/BlahST?style=flat-square) | ![Last Commit](https://img.shields.io/github/last-commit/QuantiusBenignus/BlahST?style=flat-square) | Offline, real-time, streaming speech-to-text transcription using OpenAI Whisper |
| [**blurt**](https://github.com/QuantiusBenignus/blurt) | ![Stars](https://img.shields.io/github/stars/QuantiusBenignus/blurt?style=flat-square) | ![Last Commit](https://img.shields.io/github/last-commit/QuantiusBenignus/blurt?style=flat-square) | Whisper.cpp-based STT tool |
| [**dicti**](https://github.com/tksimson/dicti) | ![Stars](https://img.shields.io/github/stars/tksimson/dicti?style=flat-square) | ![Last Commit](https://img.shields.io/github/last-commit/tksimson/dicti?style=flat-square) | Dictation tool |
| [**froshine**](https://github.com/AdrianScott/froshine) | ![Stars](https://img.shields.io/github/stars/AdrianScott/froshine?style=flat-square) | ![Last Commit](https://img.shields.io/github/last-commit/AdrianScott/froshine?style=flat-square) | Voice recognition tool |
| [**linux-stt-input**](https://github.com/fengwk/linux-stt-input) | ![Stars](https://img.shields.io/github/stars/fengwk/linux-stt-input?style=flat-square) | ![Last Commit](https://img.shields.io/github/last-commit/fengwk/linux-stt-input?style=flat-square) | Linux STT input method |
| [**linux-voice-to-text-ai**](https://github.com/trebormc/linux-voice-to-text-ai) | ![Stars](https://img.shields.io/github/stars/trebormc/linux-voice-to-text-ai?style=flat-square) | ![Last Commit](https://img.shields.io/github/last-commit/trebormc/linux-voice-to-text-ai?style=flat-square) | Linux voice to text AI |
| [**Linux-Dictation-Project**](https://github.com/wheeler01/Linux-Dictation-Project) | ![Stars](https://img.shields.io/github/stars/wheeler01/Linux-Dictation-Project?style=flat-square) | ![Last Commit](https://img.shields.io/github/last-commit/wheeler01/Linux-Dictation-Project?style=flat-square) | Linux dictation project |
| [**sonori**](https://github.com/0xPD33/sonori) | ![Stars](https://img.shields.io/github/stars/0xPD33/sonori?style=flat-square) | ![Last Commit](https://img.shields.io/github/last-commit/0xPD33/sonori?style=flat-square) | Voice recognition tool |
| [**speak-to-ai**](https://github.com/AshBuk/speak-to-ai) | ![Stars](https://img.shields.io/github/stars/AshBuk/speak-to-ai?style=flat-square) | ![Last Commit](https://img.shields.io/github/last-commit/AshBuk/speak-to-ai?style=flat-square) | Speak to AI assistant |
| [**speech-assistant**](https://github.com/Mohamad-Hussein/speech-assistant) | ![Stars](https://img.shields.io/github/stars/Mohamad-Hussein/speech-assistant?style=flat-square) | ![Last Commit](https://img.shields.io/github/last-commit/Mohamad-Hussein/speech-assistant?style=flat-square) | Faster Whisper-based speech assistant |
| [**speedofsound**](https://github.com/zugaldia/speedofsound) | ![Stars](https://img.shields.io/github/stars/zugaldia/speedofsound?style=flat-square) | ![Last Commit](https://img.shields.io/github/last-commit/zugaldia/speedofsound?style=flat-square) | Voice typing for the Linux desktop |
| [**stt-linux (afif)**](https://github.com/afif-malghani/stt-linux) | ![Stars](https://img.shields.io/github/stars/afif-malghani/stt-linux?style=flat-square) | ![Last Commit](https://img.shields.io/github/last-commit/afif-malghani/stt-linux?style=flat-square) | STT for Linux |
| [**STT-Assistant-linux**](https://github.com/4lext/STT-Assistant-linux) | ![Stars](https://img.shields.io/github/stars/4lext/STT-Assistant-linux?style=flat-square) | ![Last Commit](https://img.shields.io/github/last-commit/4lext/STT-Assistant-linux?style=flat-square) | STT assistant for Linux |
| [**super-stt**](https://github.com/jorge-menjivar/super-stt) | ![Stars](https://img.shields.io/github/stars/jorge-menjivar/super-stt?style=flat-square) | ![Last Commit](https://img.shields.io/github/last-commit/jorge-menjivar/super-stt?style=flat-square) | Enhanced STT tool |
| [**talktype**](https://github.com/lmacan1/talktype) | ![Stars](https://img.shields.io/github/stars/lmacan1/talktype?style=flat-square) | ![Last Commit](https://img.shields.io/github/last-commit/lmacan1/talktype?style=flat-square) | Push-to-talk voice typing for the terminal. Local Whisper, cross-platform |
| [**TermlAi**](https://github.com/rohitkr150015/TermlAi) | ![Stars](https://img.shields.io/github/stars/rohitkr150015/TermlAi?style=flat-square) | ![Last Commit](https://img.shields.io/github/last-commit/rohitkr150015/TermlAi?style=flat-square) | Terminal AI assistant with voice |
| [**transcribeAnywhere**](https://github.com/naren200/transcribeAnywhere) | ![Stars](https://img.shields.io/github/stars/naren200/transcribeAnywhere?style=flat-square) | ![Last Commit](https://img.shields.io/github/last-commit/naren200/transcribeAnywhere?style=flat-square) | Universal transcription tool |
| [**VocalFLow**](https://github.com/R3DK3LL/VocalFLow) | ![Stars](https://img.shields.io/github/stars/R3DK3LL/VocalFLow?style=flat-square) | ![Last Commit](https://img.shields.io/github/last-commit/R3DK3LL/VocalFLow?style=flat-square) | Voice flow dictation tool |
| [**voice-type**](https://github.com/eriknovikov/voice-type) | ![Stars](https://img.shields.io/github/stars/eriknovikov/voice-type?style=flat-square) | ![Last Commit](https://img.shields.io/github/last-commit/eriknovikov/voice-type?style=flat-square) | Linux-first system-wide dictation tool. Unmatched accuracy and speed, totally free |
| [**voicekeyboard**](https://github.com/sam1am/voicekeyboard) | ![Stars](https://img.shields.io/github/stars/sam1am/voicekeyboard?style=flat-square) | ![Last Commit](https://img.shields.io/github/last-commit/sam1am/voicekeyboard?style=flat-square) | Voice keyboard implementation |
| [**voxd**](https://github.com/jakovius/voxd) | ![Stars](https://img.shields.io/github/stars/jakovius/voxd?style=flat-square) | ![Last Commit](https://img.shields.io/github/last-commit/jakovius/voxd?style=flat-square) | Voice input daemon |
| [**whisp-away**](https://github.com/madjinn/whisp-away) | ![Stars](https://img.shields.io/github/stars/madjinn/whisp-away?style=flat-square) | ![Last Commit](https://img.shields.io/github/last-commit/madjinn/whisp-away?style=flat-square) | Whisper-based dictation tool |
| [**whisper-dictation (ananjiani)**](https://github.com/ananjiani/whisper-dictation) | ![Stars](https://img.shields.io/github/stars/ananjiani/whisper-dictation?style=flat-square) | ![Last Commit](https://img.shields.io/github/last-commit/ananjiani/whisper-dictation?style=flat-square) | Whisper-based dictation tool |
| [**whisper-hotkey-linux**](https://github.com/atkvishnu/whisper-hotkey-linux) | ![Stars](https://img.shields.io/github/stars/atkvishnu/whisper-hotkey-linux?style=flat-square) | ![Last Commit](https://img.shields.io/github/last-commit/atkvishnu/whisper-hotkey-linux?style=flat-square) | Whisper hotkey for Linux |
| [**whisper-toggle**](https://github.com/bradjmsu/whisper-toggle) | ![Stars](https://img.shields.io/github/stars/bradjmsu/whisper-toggle?style=flat-square) | ![Last Commit](https://img.shields.io/github/last-commit/bradjmsu/whisper-toggle?style=flat-square) | Toggle-based Whisper control |
| [**whisper-transcribe**](https://github.com/geraschenko/whisper-transcribe) | ![Stars](https://img.shields.io/github/stars/geraschenko/whisper-transcribe?style=flat-square) | ![Last Commit](https://img.shields.io/github/last-commit/geraschenko/whisper-transcribe?style=flat-square) | Whisper transcription tool |
| [**whisperd**](https://github.com/AgenticToaster/whisprd) | ![Stars](https://img.shields.io/github/stars/AgenticToaster/whisprd?style=flat-square) | ![Last Commit](https://img.shields.io/github/last-commit/AgenticToaster/whisprd?style=flat-square) | A daemon for OpenAI Whisper |
| [**WhisperVoice**](https://github.com/SarwadnyaMahajan/WhisperVoice) | ![Stars](https://img.shields.io/github/stars/SarwadnyaMahajan/WhisperVoice?style=flat-square) | ![Last Commit](https://img.shields.io/github/last-commit/SarwadnyaMahajan/WhisperVoice?style=flat-square) | Whisper voice processing tool |
| [**WhisperVoiceInput**](https://github.com/V0v1kkk/WhisperVoiceInput) | ![Stars](https://img.shields.io/github/stars/V0v1kkk/WhisperVoiceInput?style=flat-square) | ![Last Commit](https://img.shields.io/github/last-commit/V0v1kkk/WhisperVoiceInput?style=flat-square) | Whisper voice input tool |
| [**whispertrigger**](https://github.com/RetroTrigger/whispertrigger) | ![Stars](https://img.shields.io/github/stars/RetroTrigger/whispertrigger?style=flat-square) | ![Last Commit](https://img.shields.io/github/last-commit/RetroTrigger/whispertrigger?style=flat-square) | Trigger OpenAI Whisper with a hotkey |
| [**whispertux**](https://github.com/cjams/whispertux) | ![Stars](https://img.shields.io/github/stars/cjams/whispertux?style=flat-square) | ![Last Commit](https://img.shields.io/github/last-commit/cjams/whispertux?style=flat-square) | A simple CLI wrapper for OpenAI's Whisper speech-to-text model |
| [**wvcr**](https://github.com/bakeryproducts/wvcr) | ![Stars](https://img.shields.io/github/stars/bakeryproducts/wvcr?style=flat-square) | ![Last Commit](https://img.shields.io/github/last-commit/bakeryproducts/wvcr?style=flat-square) | Wave voice control recorder |

---

## Voice Notes & AI-Enhanced Transcription

Tools focused on capturing voice notes with AI post-processing (LLM cleanup, formatting, summarization).

| Repository | Stars | Last Updated | Description |
|------------|-------|--------------|-------------|
| [**handsfree**](https://github.com/achyudh/handsfree) | ![Stars](https://img.shields.io/github/stars/achyudh/handsfree?style=flat-square) | ![Last Commit](https://img.shields.io/github/last-commit/achyudh/handsfree?style=flat-square) | Hands-free computing |
| [**notesGPT**](https://github.com/Nutlope/notesGPT) | ![Stars](https://img.shields.io/github/stars/Nutlope/notesGPT?style=flat-square) | ![Last Commit](https://img.shields.io/github/last-commit/Nutlope/notesGPT?style=flat-square) | Voice notes with GPT processing |
| [**obsidian-scribe**](https://github.com/Mikodin/obsidian-scribe) | ![Stars](https://img.shields.io/github/stars/Mikodin/obsidian-scribe?style=flat-square) | ![Last Commit](https://img.shields.io/github/last-commit/Mikodin/obsidian-scribe?style=flat-square) | Obsidian voice note transcription |
| [**ScribeWizard**](https://github.com/Bklieger/ScribeWizard) | ![Stars](https://img.shields.io/github/stars/Bklieger/ScribeWizard?style=flat-square) | ![Last Commit](https://img.shields.io/github/last-commit/Bklieger/ScribeWizard?style=flat-square) | Transcription wizard tool |
| [**Thought-Pad**](https://github.com/danielrosehill/Thought-Pad) | ![Stars](https://img.shields.io/github/stars/danielrosehill/Thought-Pad?style=flat-square) | ![Last Commit](https://img.shields.io/github/last-commit/danielrosehill/Thought-Pad?style=flat-square) | Thought capture with STT |
| [**whisper-notes**](https://github.com/AsyncFuncAI/whisper-notes) | ![Stars](https://img.shields.io/github/stars/AsyncFuncAI/whisper-notes?style=flat-square) | ![Last Commit](https://img.shields.io/github/last-commit/AsyncFuncAI/whisper-notes?style=flat-square) | Whisper-powered note processing |
| [**whisper-notes-pro**](https://github.com/mzazakeith/whisper-notes-pro) | ![Stars](https://img.shields.io/github/stars/mzazakeith/whisper-notes-pro?style=flat-square) | ![Last Commit](https://img.shields.io/github/last-commit/mzazakeith/whisper-notes-pro?style=flat-square) | Professional whisper notes application |
| [**Whisper-Notepad-For-Linux**](https://github.com/danielrosehill/Whisper-Notepad-For-Linux) | ![Stars](https://img.shields.io/github/stars/danielrosehill/Whisper-Notepad-For-Linux?style=flat-square) | ![Last Commit](https://img.shields.io/github/last-commit/danielrosehill/Whisper-Notepad-For-Linux?style=flat-square) | Whisper notepad with post-processing |
| [**Whisper-Notepad-Simple**](https://github.com/danielrosehill/Whisper-Notepad-Simple) | ![Stars](https://img.shields.io/github/stars/danielrosehill/Whisper-Notepad-Simple?style=flat-square) | ![Last Commit](https://img.shields.io/github/last-commit/danielrosehill/Whisper-Notepad-Simple?style=flat-square) | Simplified Whisper notepad using OpenAI API |

---

## Real-Time Streaming STT

Libraries and tools for low-latency, live transcription.

| Repository | Stars | Last Updated | Description |
|------------|-------|--------------|-------------|
| [**RealtimeSTT**](https://github.com/KoljaB/RealtimeSTT) | ![Stars](https://img.shields.io/github/stars/KoljaB/RealtimeSTT?style=flat-square) | ![Last Commit](https://img.shields.io/github/last-commit/KoljaB/RealtimeSTT?style=flat-square) | Low-latency STT library with VAD, wake word activation. Uses WebRTCVAD + SileroVAD + Faster-Whisper |
| [**whisper_real_time**](https://github.com/davabase/whisper_real_time) | ![Stars](https://img.shields.io/github/stars/davabase/whisper_real_time?style=flat-square) | ![Last Commit](https://img.shields.io/github/last-commit/davabase/whisper_real_time?style=flat-square) | Real-time transcription with OpenAI Whisper |
| [**whisper_streaming**](https://github.com/ufal/whisper_streaming) | ![Stars](https://img.shields.io/github/stars/ufal/whisper_streaming?style=flat-square) | ![Last Commit](https://img.shields.io/github/last-commit/ufal/whisper_streaming?style=flat-square) | Real-time streaming Whisper with self-adaptive latency using local agreement policy |
| [**WhisperLive**](https://github.com/collabora/WhisperLive) | ![Stars](https://img.shields.io/github/stars/collabora/WhisperLive?style=flat-square) | ![Last Commit](https://img.shields.io/github/last-commit/collabora/WhisperLive?style=flat-square) | Real-time Whisper transcription from Collabora. OpenVINO support, browser extensions, iOS client |
| [**WhisperLiveKit**](https://github.com/QuentinFuxa/WhisperLiveKit) | ![Stars](https://img.shields.io/github/stars/QuentinFuxa/WhisperLiveKit?style=flat-square) | ![Last Commit](https://img.shields.io/github/last-commit/QuentinFuxa/WhisperLiveKit?style=flat-square) | 2025 SOTA streaming STT with speaker diarization. Simul-Whisper for ultra-low latency |

---

## Self-Hosted / Web UI

Docker-deployed tools and web interfaces for self-hosted STT.

| Repository | Stars | Last Updated | Description |
|------------|-------|--------------|-------------|
| [**meeting-minutes**](https://github.com/Zackriya-Solutions/meeting-minutes) | ![Stars](https://img.shields.io/github/stars/Zackriya-Solutions/meeting-minutes?style=flat-square) | ![Last Commit](https://img.shields.io/github/last-commit/Zackriya-Solutions/meeting-minutes?style=flat-square) | Self-hostable meeting transcription and minutes generation |
| [**Scriberr**](https://github.com/rishikanthc/Scriberr) | ![Stars](https://img.shields.io/github/stars/rishikanthc/Scriberr?style=flat-square) | ![Last Commit](https://img.shields.io/github/last-commit/rishikanthc/Scriberr?style=flat-square) | Voice transcription tool |
| [**Whisper-WebUI**](https://github.com/jhj0517/Whisper-WebUI) | ![Stars](https://img.shields.io/github/stars/jhj0517/Whisper-WebUI?style=flat-square) | ![Last Commit](https://img.shields.io/github/last-commit/jhj0517/Whisper-WebUI?style=flat-square) | A Gradio-based browser interface for Whisper. Easy subtitle generation |
| [**whisper-fastapi**](https://github.com/heimoshuiyu/whisper-fastapi) | ![Stars](https://img.shields.io/github/stars/heimoshuiyu/whisper-fastapi?style=flat-square) | ![Last Commit](https://img.shields.io/github/last-commit/heimoshuiyu/whisper-fastapi?style=flat-square) | Whisper FastAPI service |

---

## Cloud STT / API-Based Tools

Projects that use cloud STT APIs for transcription.

### OpenAI Whisper API

| Repository | Stars | Last Updated | Description |
|------------|-------|--------------|-------------|
| [**speech2keys**](https://github.com/vanviegen/speech2keys) | ![Stars](https://img.shields.io/github/stars/vanviegen/speech2keys?style=flat-square) | ![Last Commit](https://img.shields.io/github/last-commit/vanviegen/speech2keys?style=flat-square) | Speech to keystrokes using OpenAI Whisper API |

### Deepgram API

| Repository | Stars | Last Updated | Description |
|------------|-------|--------------|-------------|
| [**Deepgram-Voice-Keyboard-Ubuntu**](https://github.com/danielrosehill/Deepgram-Voice-Keyboard-Ubuntu) | ![Stars](https://img.shields.io/github/stars/danielrosehill/Deepgram-Voice-Keyboard-Ubuntu?style=flat-square) | ![Last Commit](https://img.shields.io/github/last-commit/danielrosehill/Deepgram-Voice-Keyboard-Ubuntu?style=flat-square) | STT project using Deepgram API for Ubuntu |
| [**fortuna**](https://github.com/deepgram-devs/fortuna) | ![Stars](https://img.shields.io/github/stars/deepgram-devs/fortuna?style=flat-square) | ![Last Commit](https://img.shields.io/github/last-commit/deepgram-devs/fortuna?style=flat-square) | Deepgram Fortuna project |
| [**voice-keyboard-linux**](https://github.com/deepgram/voice-keyboard-linux) | ![Stars](https://img.shields.io/github/stars/deepgram/voice-keyboard-linux?style=flat-square) | ![Last Commit](https://img.shields.io/github/last-commit/deepgram/voice-keyboard-linux?style=flat-square) | Deepgram voice keyboard for Linux |

### Hugging Face ASR Models

| Resource | Description |
|----------|-------------|
| [ASR Models (Trending)](https://huggingface.co/models?pipeline_tag=automatic-speech-recognition&sort=trending) | Trending automatic speech recognition models on Hugging Face |
| [Whisper on Hugging Face](https://huggingface.co/spaces/openai/whisper) | OpenAI Whisper on Hugging Face |

---

## Voice Assistants

### Privacy-Focused

Open source voice assistants emphasizing local processing and privacy.

| Repository | Stars | Last Updated | Description |
|------------|-------|--------------|-------------|
| [**Neon AI**](https://github.com/NeonGeckoCom/NeonCore) | ![Stars](https://img.shields.io/github/stars/NeonGeckoCom/NeonCore?style=flat-square) | ![Last Commit](https://img.shields.io/github/last-commit/NeonGeckoCom/NeonCore?style=flat-square) | Privacy-first voice assistant. Offline-capable, customizable. Maintains Mycroft community forums |
| [**OpenVoiceOS**](https://github.com/OpenVoiceOS/ovos-core) | ![Stars](https://img.shields.io/github/stars/OpenVoiceOS/ovos-core?style=flat-square) | ![Last Commit](https://img.shields.io/github/last-commit/OpenVoiceOS/ovos-core?style=flat-square) | Community-driven voice assistant framework. Local processing, privacy-focused. Continuation of Mycroft |
| [**Project Alice**](https://github.com/project-alice-assistant/ProjectAlice) | ![Stars](https://img.shields.io/github/stars/project-alice-assistant/ProjectAlice?style=flat-square) | ![Last Commit](https://img.shields.io/github/last-commit/project-alice-assistant/ProjectAlice?style=flat-square) | Modular smart assistant, fully offline. Built around Snips, guarantees privacy |
| [**SEPIA Framework**](https://github.com/SEPIA-Framework/sepia-assist-server) | ![Stars](https://img.shields.io/github/stars/SEPIA-Framework/sepia-assist-server?style=flat-square) | ![Last Commit](https://img.shields.io/github/last-commit/SEPIA-Framework/sepia-assist-server?style=flat-square) | Self-hosted, privacy-compliant voice assistant ecosystem |

### General

| Repository | Stars | Last Updated | Description |
|------------|-------|--------------|-------------|
| [**jarvis_linux**](https://github.com/morrolinux/jarvis_linux) | ![Stars](https://img.shields.io/github/stars/morrolinux/jarvis_linux?style=flat-square) | ![Last Commit](https://img.shields.io/github/last-commit/morrolinux/jarvis_linux?style=flat-square) | Jarvis for Linux |
| [**linux-voice-control**](https://github.com/omegaui/linux-voice-control) | ![Stars](https://img.shields.io/github/stars/omegaui/linux-voice-control?style=flat-square) | ![Last Commit](https://img.shields.io/github/last-commit/omegaui/linux-voice-control?style=flat-square) | Linux voice control system |
| [**LinuxVoiceAssistant**](https://github.com/aydinnyunus/LinuxVoiceAssistant) | ![Stars](https://img.shields.io/github/stars/aydinnyunus/LinuxVoiceAssistant?style=flat-square) | ![Last Commit](https://img.shields.io/github/last-commit/aydinnyunus/LinuxVoiceAssistant?style=flat-square) | Linux voice assistant |
| [**Local-Voice**](https://github.com/shashank2122/Local-Voice) | ![Stars](https://img.shields.io/github/stars/shashank2122/Local-Voice?style=flat-square) | ![Last Commit](https://img.shields.io/github/last-commit/shashank2122/Local-Voice?style=flat-square) | Local voice assistant |
| [**Personal-Voice-Assistent**](https://github.com/Cyborgscode/Personal-Voice-Assistent) | ![Stars](https://img.shields.io/github/stars/Cyborgscode/Personal-Voice-Assistent?style=flat-square) | ![Last Commit](https://img.shields.io/github/last-commit/Cyborgscode/Personal-Voice-Assistent?style=flat-square) | Personal voice assistant |
| [**tempest**](https://github.com/lavafroth/tempest) | ![Stars](https://img.shields.io/github/stars/lavafroth/tempest?style=flat-square) | ![Last Commit](https://img.shields.io/github/last-commit/lavafroth/tempest?style=flat-square) | Voice assistant framework |
| [**vosk-cli-dictation**](https://github.com/RonanDavalan/vosk-cli-dictation) | ![Stars](https://img.shields.io/github/stars/RonanDavalan/vosk-cli-dictation?style=flat-square) | ![Last Commit](https://img.shields.io/github/last-commit/RonanDavalan/vosk-cli-dictation?style=flat-square) | Vosk CLI dictation |

---

## Voice Commands & Automation

Tools that translate voice into actions — computer control, voice-to-commands, voice-to-JSON, etc.

| Repository | Stars | Last Updated | Description |
|------------|-------|--------------|-------------|
| [**Handy**](https://github.com/cjpais/Handy) | ![Stars](https://img.shields.io/github/stars/cjpais/Handy?style=flat-square) | ![Last Commit](https://img.shields.io/github/last-commit/cjpais/Handy?style=flat-square) | Voice-controlled computer interface - [handy.computer](https://handy.computer/) |
| [**home-assistant-assist-desktop**](https://github.com/timmo001/home-assistant-assist-desktop) | ![Stars](https://img.shields.io/github/stars/timmo001/home-assistant-assist-desktop?style=flat-square) | ![Last Commit](https://img.shields.io/github/last-commit/timmo001/home-assistant-assist-desktop?style=flat-square) | Home Assistant desktop client |
| [**JustSayIt.jl**](https://github.com/omlins/JustSayIt.jl) | ![Stars](https://img.shields.io/github/stars/omlins/JustSayIt.jl?style=flat-square) | ![Last Commit](https://img.shields.io/github/last-commit/omlins/JustSayIt.jl?style=flat-square) | Offline, low-latency translation of speech to computer commands or text. Julia-based |
| [**numen**](https://sr.ht/~geb/numen/) | N/A | N/A | Voice-controlled interface (hosted on SourceHut) |
| [**voice2json**](https://github.com/synesthesiam/voice2json) | ![Stars](https://img.shields.io/github/stars/synesthesiam/voice2json?style=flat-square) | ![Last Commit](https://img.shields.io/github/last-commit/synesthesiam/voice2json?style=flat-square) | Voice to JSON converter |

---

## Voice Operating Systems

| Repository | Stars | Last Updated | Description |
|------------|-------|--------------|-------------|
| [**ovos-buildroot**](https://github.com/OpenVoiceOS/ovos-buildroot) | ![Stars](https://img.shields.io/github/stars/OpenVoiceOS/ovos-buildroot?style=flat-square) | ![Last Commit](https://img.shields.io/github/last-commit/OpenVoiceOS/ovos-buildroot?style=flat-square) | OpenVoiceOS - A minimalistic Linux OS bringing the open source voice assistant to IoT and embedded devices |

---

## Subtitle Generation

| Repository | Stars | Last Updated | Description |
|------------|-------|--------------|-------------|
| [**auto-subs**](https://github.com/tmoroney/auto-subs) | ![Stars](https://img.shields.io/github/stars/tmoroney/auto-subs?style=flat-square) | ![Last Commit](https://img.shields.io/github/last-commit/tmoroney/auto-subs?style=flat-square) | Automatic subtitle generation |
| [**whisper-subs**](https://github.com/GhostNaN/whisper-subs) | ![Stars](https://img.shields.io/github/stars/GhostNaN/whisper-subs?style=flat-square) | ![Last Commit](https://img.shields.io/github/last-commit/GhostNaN/whisper-subs?style=flat-square) | Whisper subtitle generation |

---

## Service-Specific Voice Tools

| Repository | Stars | Last Updated | Description |
|------------|-------|--------------|-------------|
| [**deepin-voice-note**](https://github.com/linuxdeepin/deepin-voice-note) | ![Stars](https://img.shields.io/github/stars/linuxdeepin/deepin-voice-note?style=flat-square) | ![Last Commit](https://img.shields.io/github/last-commit/linuxdeepin/deepin-voice-note?style=flat-square) | Deepin voice note application |
| [**overlayed**](https://github.com/overlayeddev/overlayed) | ![Stars](https://img.shields.io/github/stars/overlayeddev/overlayed?style=flat-square) | ![Last Commit](https://img.shields.io/github/last-commit/overlayeddev/overlayed?style=flat-square) | Voice overlay for Discord on Linux |
| [**whatsapp_voice_transcription**](https://github.com/nerveband/whatsapp_voice_transcription) | ![Stars](https://img.shields.io/github/stars/nerveband/whatsapp_voice_transcription?style=flat-square) | ![Last Commit](https://img.shields.io/github/last-commit/nerveband/whatsapp_voice_transcription?style=flat-square) | WhatsApp voice message transcription |

---

## Voice Biometrics

| Repository | Stars | Last Updated | Description |
|------------|-------|--------------|-------------|
| [**voiceprint**](https://github.com/Raymo111/voiceprint) | ![Stars](https://img.shields.io/github/stars/Raymo111/voiceprint?style=flat-square) | ![Last Commit](https://img.shields.io/github/last-commit/Raymo111/voiceprint?style=flat-square) | Voice biometric authentication for Linux |

---

## Developer Tools

| Repository | Stars | Last Updated | Description |
|------------|-------|--------------|-------------|
| [**mt_stt**](https://github.com/RhinoDevel/mt_stt) | ![Stars](https://img.shields.io/github/stars/RhinoDevel/mt_stt?style=flat-square) | ![Last Commit](https://img.shields.io/github/last-commit/RhinoDevel/mt_stt?style=flat-square) | C wrapper for speech-to-text |
| [**whisper.cpp-cli**](https://github.com/charliermarsh/whisper.cpp-cli) | ![Stars](https://img.shields.io/github/stars/charliermarsh/whisper.cpp-cli?style=flat-square) | ![Last Commit](https://img.shields.io/github/last-commit/charliermarsh/whisper.cpp-cli?style=flat-square) | Whisper.cpp CLI wrapper |
| [**whisper** (Nutlope)](https://github.com/Nutlope/whisper) | ![Stars](https://img.shields.io/github/stars/Nutlope/whisper?style=flat-square) | ![Last Commit](https://img.shields.io/github/last-commit/Nutlope/whisper?style=flat-square) | Whisper implementation |

### Proof of Concepts

| Repository | Stars | Last Updated | Description |
|------------|-------|--------------|-------------|
| [**stt-linux (samcole8)**](https://github.com/samcole8/stt-linux) | ![Stars](https://img.shields.io/github/stars/samcole8/stt-linux?style=flat-square) | ![Last Commit](https://img.shields.io/github/last-commit/samcole8/stt-linux?style=flat-square) | STT Linux proof of concept |
| [**whisperai**](https://github.com/jorgecastro05/whisperai) | ![Stars](https://img.shields.io/github/stars/jorgecastro05/whisperai?style=flat-square) | ![Last Commit](https://img.shields.io/github/last-commit/jorgecastro05/whisperai?style=flat-square) | Whisper AI proof of concept |

---

## Complementary Tools

Tools that aren't STT themselves, but help make the most of voice workflows.

### Noise Suppression & Audio Processing

| Repository | Stars | Last Updated | Description |
|------------|-------|--------------|-------------|
| [**easyeffects**](https://github.com/wwmm/easyeffects) | ![Stars](https://img.shields.io/github/stars/wwmm/easyeffects?style=flat-square) | ![Last Commit](https://img.shields.io/github/last-commit/wwmm/easyeffects?style=flat-square) | Audio effects for PipeWire applications - noise reduction, equalization, and more |
| [**NoiseTorch**](https://github.com/noisetorch/NoiseTorch) | ![Stars](https://img.shields.io/github/stars/noisetorch/NoiseTorch?style=flat-square) | ![Last Commit](https://img.shields.io/github/last-commit/noisetorch/NoiseTorch?style=flat-square) | Real-time microphone noise suppression on Linux |

### Voice Activity Detection (VAD) & Diarisation

| Repository | Stars | Last Updated | Description |
|------------|-------|--------------|-------------|
| [**pyannote-audio**](https://github.com/pyannote/pyannote-audio) | ![Stars](https://img.shields.io/github/stars/pyannote/pyannote-audio?style=flat-square) | ![Last Commit](https://img.shields.io/github/last-commit/pyannote/pyannote-audio?style=flat-square) | Neural building blocks for speaker diarization: speech activity detection, speaker embedding, clustering |
| [**Silero VAD**](https://github.com/snakers4/silero-vad) | ![Stars](https://img.shields.io/github/stars/snakers4/silero-vad?style=flat-square) | ![Last Commit](https://img.shields.io/github/last-commit/snakers4/silero-vad?style=flat-square) | Enterprise-grade Voice Activity Detector. MIT license, <1ms per chunk on CPU |
| [**WebRTC VAD**](https://github.com/wiseman/py-webrtcvad) | ![Stars](https://img.shields.io/github/stars/wiseman/py-webrtcvad?style=flat-square) | ![Last Commit](https://img.shields.io/github/last-commit/wiseman/py-webrtcvad?style=flat-square) | Python interface to WebRTC Voice Activity Detector |
| [**wyoming-openwakeword**](https://github.com/rhasspy/wyoming-openwakeword) | ![Stars](https://img.shields.io/github/stars/rhasspy/wyoming-openwakeword?style=flat-square) | ![Last Commit](https://img.shields.io/github/last-commit/rhasspy/wyoming-openwakeword?style=flat-square) | Custom wake word detection for Home Assistant |

---

## Toolkits & Frameworks

ASR/STT toolkits and frameworks for building voice applications. Developer libraries rather than end-user applications.

| Repository | Stars | Last Updated | Description |
|------------|-------|--------------|-------------|
| [**Coqui STT**](https://github.com/coqui-ai/STT) | ![Stars](https://img.shields.io/github/stars/coqui-ai/STT?style=flat-square) | ![Last Commit](https://img.shields.io/github/last-commit/coqui-ai/STT?style=flat-square) | Deep learning STT toolkit (continuation of Mozilla DeepSpeech). Custom model training |
| [**fairseq**](https://github.com/facebookresearch/fairseq) | ![Stars](https://img.shields.io/github/stars/facebookresearch/fairseq?style=flat-square) | ![Last Commit](https://img.shields.io/github/last-commit/facebookresearch/fairseq?style=flat-square) | Meta's sequence modeling toolkit. Includes Wav2Vec 2.0 for self-supervised ASR |
| [**FunASR**](https://github.com/modelscope/FunASR) | ![Stars](https://img.shields.io/github/stars/modelscope/FunASR?style=flat-square) | ![Last Commit](https://img.shields.io/github/last-commit/modelscope/FunASR?style=flat-square) | End-to-end speech recognition toolkit from Alibaba. Industrial-grade models |
| [**NVIDIA NeMo**](https://github.com/NVIDIA/NeMo) | ![Stars](https://img.shields.io/github/stars/NVIDIA/NeMo?style=flat-square) | ![Last Commit](https://img.shields.io/github/last-commit/NVIDIA/NeMo?style=flat-square) | Enterprise ASR toolkit with Conformer/Parakeet models. GPU-accelerated training and inference |
| [**sherpa-onnx**](https://github.com/k2-fsa/sherpa-onnx) | ![Stars](https://img.shields.io/github/stars/k2-fsa/sherpa-onnx?style=flat-square) | ![Last Commit](https://img.shields.io/github/last-commit/k2-fsa/sherpa-onnx?style=flat-square) | STT, TTS, speaker diarization, VAD using next-gen Kaldi with ONNX Runtime. Offline, 12 programming languages |
| [**sherpa-onnx-go**](https://github.com/k2-fsa/sherpa-onnx-go) | ![Stars](https://img.shields.io/github/stars/k2-fsa/sherpa-onnx-go?style=flat-square) | ![Last Commit](https://img.shields.io/github/last-commit/k2-fsa/sherpa-onnx-go?style=flat-square) | Go package for sherpa-onnx speech recognition without network access |
| [**SpeechBrain**](https://github.com/speechbrain/speechbrain) | ![Stars](https://img.shields.io/github/stars/speechbrain/speechbrain?style=flat-square) | ![Last Commit](https://img.shields.io/github/last-commit/speechbrain/speechbrain?style=flat-square) | PyTorch-based speech toolkit for ASR, speaker recognition, speech enhancement |
| [**Vosk**](https://github.com/alphacep/vosk-api) | ![Stars](https://img.shields.io/github/stars/alphacep/vosk-api?style=flat-square) | ![Last Commit](https://img.shields.io/github/last-commit/alphacep/vosk-api?style=flat-square) | Offline speech recognition API. Lightweight, 20+ languages, works on Raspberry Pi |

---

## Whisper Variants & Optimizations

Optimized implementations and variants of OpenAI's Whisper model.

| Repository | Stars | Last Updated | Description |
|------------|-------|--------------|-------------|
| [**distil-whisper**](https://github.com/huggingface/distil-whisper) | ![Stars](https://img.shields.io/github/stars/huggingface/distil-whisper?style=flat-square) | ![Last Commit](https://img.shields.io/github/last-commit/huggingface/distil-whisper?style=flat-square) | HuggingFace's distilled Whisper. 6x faster, 49% smaller, within 1% WER |
| [**faster-whisper**](https://github.com/SYSTRAN/faster-whisper) | ![Stars](https://img.shields.io/github/stars/SYSTRAN/faster-whisper?style=flat-square) | ![Last Commit](https://img.shields.io/github/last-commit/SYSTRAN/faster-whisper?style=flat-square) | CTranslate2 reimplementation. 4x faster, less memory, 8-bit quantization support |
| [**insanely-fast-whisper**](https://github.com/Vaibhavs10/insanely-fast-whisper) | ![Stars](https://img.shields.io/github/stars/Vaibhavs10/insanely-fast-whisper?style=flat-square) | ![Last Commit](https://img.shields.io/github/last-commit/Vaibhavs10/insanely-fast-whisper?style=flat-square) | CLI for fastest Whisper inference. Batching, flash attention, distil-whisper support |
| [**whisper.cpp**](https://github.com/ggerganov/whisper.cpp) | ![Stars](https://img.shields.io/github/stars/ggerganov/whisper.cpp?style=flat-square) | ![Last Commit](https://img.shields.io/github/last-commit/ggerganov/whisper.cpp?style=flat-square) | C/C++ port of Whisper. CPU inference, minimal dependencies, runs on edge devices |
| [**whisper-plus**](https://github.com/kadirnar/whisper-plus) | ![Stars](https://img.shields.io/github/stars/kadirnar/whisper-plus?style=flat-square) | ![Last Commit](https://img.shields.io/github/last-commit/kadirnar/whisper-plus?style=flat-square) | Advanced Whisper pipelines with diarization, translation, and video transcription support |
| [**wyoming-faster-whisper**](https://github.com/rhasspy/wyoming-faster-whisper) | ![Stars](https://img.shields.io/github/stars/rhasspy/wyoming-faster-whisper?style=flat-square) | ![Last Commit](https://img.shields.io/github/last-commit/rhasspy/wyoming-faster-whisper?style=flat-square) | Wyoming protocol server for faster-whisper. Home Assistant integration |
| [**wyoming-whisper-api-client**](https://github.com/ser/wyoming-whisper-api-client) | ![Stars](https://img.shields.io/github/stars/ser/wyoming-whisper-api-client?style=flat-square) | ![Last Commit](https://img.shields.io/github/last-commit/ser/wyoming-whisper-api-client?style=flat-square) | Wyoming protocol client for Whisper APIs. Centralizes STT for Home Assistant |

---

## Text-to-Speech (TTS)

| Repository | Stars | Last Updated | Description |
|------------|-------|--------------|-------------|
| [**claude-tts**](https://github.com/MatiousCorp/claude-tts) | ![Stars](https://img.shields.io/github/stars/MatiousCorp/claude-tts?style=flat-square) | ![Last Commit](https://img.shields.io/github/last-commit/MatiousCorp/claude-tts?style=flat-square) | TTS plugin for Claude Code — multi-provider support (ElevenLabs, OpenAI, Google, Amazon Polly, Azure, local system TTS) |

---

## MCP Servers

MCP (Model Context Protocol) servers that provide STT capabilities.

| Repository | Stars | Last Updated | Description |
|------------|-------|--------------|-------------|
| [**stt-mcp-server-linux**](https://github.com/marcindulak/stt-mcp-server-linux) | ![Stars](https://img.shields.io/github/stars/marcindulak/stt-mcp-server-linux?style=flat-square) | ![Last Commit](https://img.shields.io/github/last-commit/marcindulak/stt-mcp-server-linux?style=flat-square) | Local speech-to-text MCP server for Tmux on Linux (for use with Claude Code and other MCP clients) |

---

## Awesome Lists

| Repository | Stars | Last Updated | Description |
|------------|-------|--------------|-------------|
| [**awesome-voice-typing**](https://github.com/primaprashant/awesome-voice-typing) | ![Stars](https://img.shields.io/github/stars/primaprashant/awesome-voice-typing?style=flat-square) | ![Last Commit](https://img.shields.io/github/last-commit/primaprashant/awesome-voice-typing?style=flat-square) | Curated list of open-source STT and voice typing tools for Linux, macOS, Windows, Android, and iOS |
| [**Voice-Apps-Index**](https://github.com/danielrosehill/Voice-Apps-Index) | ![Stars](https://img.shields.io/github/stars/danielrosehill/Voice-Apps-Index?style=flat-square) | ![Last Commit](https://img.shields.io/github/last-commit/danielrosehill/Voice-Apps-Index?style=flat-square) | Index for STT and dictation apps and WIPs |

---

## Ideas & Specifications

Projects at the concept or specification stage.

| Repository | Stars | Last Updated | Description |
|------------|-------|--------------|-------------|
| [**VoiceBox**](https://github.com/danielrosehill/VoiceBox) | ![Stars](https://img.shields.io/github/stars/danielrosehill/VoiceBox?style=flat-square) | ![Last Commit](https://img.shields.io/github/last-commit/danielrosehill/VoiceBox?style=flat-square) | Idea for a speech tech solution — specced out by Claude |

---

## Archived Projects

Notable projects that are no longer actively maintained.

| Repository | Stars | Last Updated | Description |
|------------|-------|--------------|-------------|
| [**AI-Transcription-Notepad**](https://github.com/danielrosehill/AI-Transcription-Notepad) | ![Stars](https://img.shields.io/github/stars/danielrosehill/AI-Transcription-Notepad?style=flat-square) | ![Last Commit](https://img.shields.io/github/last-commit/danielrosehill/AI-Transcription-Notepad?style=flat-square) | Voice note taking utility using cloud audio multimodal models for single-pass transcription and text cleanup (archived) |

---

## Community Resources

### GitHub Topics

| Topic | Description |
|-------|-------------|
| [asr](https://github.com/topics/asr) | Automatic speech recognition |
| [dictation](https://github.com/topics/dictation) | Dictation tools and applications |
| [speech-to-text](https://github.com/topics/speech-to-text) | General speech-to-text projects |
| [transcription](https://github.com/topics/transcription) | Audio/video transcription tools |
| [voice](https://github.com/topics/voice) | General voice technology projects |
| [voice-assistant](https://github.com/topics/voice-assistant) | Voice assistant applications |
| [voice-commands](https://github.com/topics/voice-commands) | Voice command implementations |
| [voice-control](https://github.com/topics/voice-control) | Voice control tools |
| [voice-dictation](https://github.com/topics/voice-dictation) | Voice dictation specific projects |
| [voice-recognition](https://github.com/topics/voice-recognition) | Voice recognition systems |

### Subreddits

| Subreddit | Focus |
|-----------|-------|
| [r/accessibility](https://www.reddit.com/r/accessibility/) | Accessibility tools including voice control |
| [r/LocalLLaMA](https://www.reddit.com/r/LocalLLaMA/) | Local LLMs (frequently covers voice topics) |
| [r/opensource](https://www.reddit.com/r/opensource/) | Open source projects including voice tools |
| [r/speechrecognition](https://www.reddit.com/r/speechrecognition/) | Speech recognition systems and discussion |
| [r/TextToSpeech](https://www.reddit.com/r/TextToSpeech/) | TTS technology (complementary to STT) |
| [r/VoiceTech](https://www.reddit.com/r/VoiceTech/) | Voice technology and applications |
