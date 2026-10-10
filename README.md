# qalun-models

The speech recognition model Qalun downloads once, on first use, to transcribe
Arabic audio on the user's own computer.

| Release | File | Model |
|---|---|---|
| `model-v1` | `stt_ar_fastconformer_hybrid_large_pcd_v1.0-int8-1.tar.bz2` (108 MB) | NVIDIA FastConformer Hybrid Large (Arabic), transducer branch, int8, for sherpa-onnx |

Qalun pins each file's SHA-256 and refuses anything that does not match. A
published asset is therefore never replaced in place: a new model is a new
release, and a new Qalun version points to it.

## Licence and attribution

The model is NVIDIA's `stt_ar_fastconformer_hybrid_large_pcd_v1.0`
(https://huggingface.co/nvidia/stt_ar_fastconformer_hybrid_large_pcd_v1.0),
© NVIDIA Corporation, licensed under Creative Commons Attribution 4.0
International (CC BY 4.0): https://creativecommons.org/licenses/by/4.0/.

Changes made: converted to ONNX for sherpa-onnx (transducer branch only), with
the weights quantised to 8 bits. See `NOTICE.md` in each release.
