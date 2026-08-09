# Echotools Runtime

Downloadable runtime assets for the [EchoTools](https://github.com/pigon-ai) VS Code extensions — voice models and supporting data that are too large to ship inside the extension packages.

Extensions fetch these files **once, with your consent, over HTTPS** — and verify every download against a SHA-256 digest and exact byte size pinned in the extension's source. A file that does not match is discarded, never used.

## Releases

| tag | contents | license |
|---|---|---|
| `kokoro-v1` | Kokoro TTS: 82M quantized ONNX model + 29 voice embeddings | Apache-2.0 (source: [onnx-community/Kokoro-82M-v1.0-ONNX](https://huggingface.co/onnx-community/Kokoro-82M-v1.0-ONNX), base model hexgrad/Kokoro-82M) |

This repository hosts **data, not code**. The extensions' code ships in their marketplace packages; their documentation lives at [pigon-ai/echovoice](https://github.com/pigon-ai/echovoice) and [pigon-ai/echoavatar](https://github.com/pigon-ai/echoavatar).

Contact: milo@pigon.ai
