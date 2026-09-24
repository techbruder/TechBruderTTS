# TechBruderTTS — Mobile On-Device TTS Runtime & Assets

High-performance, on-device neural text-to-speech runtime assets and configurations optimized for mobile execution via ONNX Runtime on Android and iOS.

---

## Overview

TechBruderTTS provides the binary lookup matrices, tokenizer artifacts, and model delivery configuration required to execute local, quantized speech synthesis on edge hardware without cloud latency or external API dependencies.

### Key Capabilities
* **Offline First:** Zero telemetry or cloud dependencies for audio synthesis.
* **Quantized Architecture:** Optimized INT8/FP16 pipelines tailored for low memory footprints on modern mobile chips.
* **Streaming Vocoder Support:** Direct frame-by-frame decoding designed for low-latency PCM playback.

---

## Repository Structure

```text
├── models/
│   └── alibaba_Qwen3-TTS-1.7B/
│       ├── tokenizer.json          # Tokenizer vocabulary & configuration
│       ├── vocab.json              # Direct token map
│       └── embed_tokens.bin        # Pre-computed float token embedding matrix
├── manifests/
│   └── model_manifest.json         # Checksums, sizes, and remote asset endpoints
└── README.md
