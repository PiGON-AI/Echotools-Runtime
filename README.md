# Echotools Runtime

Downloadable runtime assets for the [EchoTools](https://github.com/pigon-ai) VS Code extensions — voice models and supporting data that are too large to ship inside the extension packages.

Extensions fetch these files **once, with your consent, over HTTPS** — and verify every download against a SHA-256 digest and exact byte size pinned in the extension's source. A file that does not match is discarded, never used.

## Releases

| tag | contents | license |
|---|---|---|
| `kokoro-v1` | Kokoro TTS: 82M quantized ONNX model + 29 voice embeddings | Apache-2.0 (source: [onnx-community/Kokoro-82M-v1.0-ONNX](https://huggingface.co/onnx-community/Kokoro-82M-v1.0-ONNX), base model hexgrad/Kokoro-82M) |
| `whisper-v1` | Speech to text for the push-to-talk button: whisper.cpp command-line binaries for Windows x64, macOS arm64 and Linux x64, built by this repository's own workflow from one pinned upstream commit, plus the English base model | MIT (whisper.cpp), MIT (model, derived from OpenAI Whisper) |

This repository hosts **data, and the build recipes that produce it** (`.github/workflows/`), never the extensions' code. The extensions' code ships in their marketplace packages; their documentation lives at [pigon-ai/echovoice](https://github.com/pigon-ai/echovoice) and [pigon-ai/echoavatar](https://github.com/pigon-ai/echoavatar).

Contact: milo@pigon.ai
