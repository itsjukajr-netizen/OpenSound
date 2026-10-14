# OpenSound

Created by **Preston Harmon**.

OpenSound is a Windows desktop audio workstation for music, sound editing for film, voice cloning and effects.

## Download

**[Download OpenSound for Windows x64](https://github.com/itsjukajr-netizen/OpenSound/releases/download/v0.1.0-alpha.1/OpenSound-0.1.0-alpha.1-Windows-x64-setup.exe)**

Run the installer, then open OpenSound. Requires Windows 10/11 x64 and the Microsoft Edge WebView2 Runtime. This is a development alpha. See [Releases](https://github.com/itsjukajr-netizen/OpenSound/releases) for release notes and checksums.

This repository distributes the app and its documentation. Application source code is maintained locally and is not included in the current repository files.

## Inside the app

- **Music:** import and mix audio, edit clips and MIDI notes, use automation and export mixes or stems.
- **Film:** edit dialogue, ambience and other sound for film. Video playback and timecode are not included.
- **Voice Cloning:** generate speech or clone a reference voice locally with optional Qwen3-TTS; optional Whisper transcription is also available.
- **Effects:** EQ, compression, gates, delay, reverb, limiting, buses and sends.

Sessions process at 48 kHz with stereo output. Import mono/stereo WAV at 44.1/48/96 kHz, or FLAC, MP3 and Ogg Vorbis at 44.1/48 kHz. Export float32, PCM16 or PCM24 WAV.

Choose **Open demo**, or create a session and import audio. Select an output device and press Space to play or pause. Ctrl+S saves. Recording starts only through the recording controls.

Local AI features need an existing Python with pip to bootstrap their separate runtime/model setup, internet access and several GB of disk; normal mixing does not require them. Setup instructions and scripts accompany the Windows app. Hardware compatibility, native workflows and clean-machine installation still need broader qualification.

## Updates

Choose **Help → Check for updates → Download & update**. OpenSound saves your session, verifies the signed update, installs it and restarts automatically. Stop playback or recording first. You can cancel before installation starts. Songs and sessions are retained, and the previous executable is kept as a recovery copy.

## Credits and licenses

OpenSound uses Rust, Tauri and its updater, Symphonia, CPAL, Rubato, Hound, TypeScript, Vite and other open-source libraries. Optional local tools use Qwen3-TTS, Demucs and Whisper. Thank you to their authors and maintainers.

See [credits](CREDITS.md), [dependencies](docs/dependencies.md) and the [MIT license](LICENSE). The Windows app includes third-party license notices, exact package versions and corresponding source archives for MPL-2.0 components. Original third-party copyrights and licenses remain in effect.

Your songs, recordings, sessions, exports, model weights and private test files are not uploaded to this repository or included in downloads.
