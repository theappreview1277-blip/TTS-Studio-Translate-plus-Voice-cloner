# TTS-Studio-Translate-plus-Voice-cloner
 An open-source, offline-first text-to-speech and translation studio for Windows — translate documents section by section and read them aloud with Piper, Kokoro, or Chatterbox voice cloning.
TTS Studio is an open-source, modular desktop app for Windows that turns written documents into spoken audio, with offline translation built in along the way. Paste or import a `.txt`, `.md`, `.docx`, or `.pdf`, split it into sections, translate each one independently with Argos Translate (fully offline, no server calls), and generate speech section by section — editing, regenerating, or re-translating any single section without redoing the whole document.

Three text-to-speech engines are included, each exposing only the controls it actually supports:

- **Piper** and **Kokoro** — fast, fully offline neural voices with speed, volume, and (for Kokoro) character-blend presets.
- **Chatterbox** — voice cloning from a short reference clip, in three model tiers (Nano, Turbo, Original) for CPU or GPU use, with its own native expression, guidance, and sampling controls.

Everything runs locally: no cloud APIs, no accounts, no per-word pricing. A one-click Windows installer sets up Python, FFmpeg, espeak-ng, and every model dependency automatically, including Chatterbox's separate environment (kept isolated so its dependencies don't conflict with the rest of the app). Finished audio exports to WAV, MP3, FLAC, or OGG, and full projects — source text, translations, per-section audio, and settings — save and reload as a single folder.

Licensing is intentionally kept clean and inspectable: Piper (GPL-3.0) runs as an isolated subprocess rather than being linked in-process, Kokoro and Argos Translate are permissively licensed, and Chatterbox's code and model weights are both MIT.
