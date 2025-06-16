
# Benchmarks

How it works:
- Start TrustGraph
- Load the Challenger report volume 1
- Submit with the default flow
- Monitor the throughput in Grafana.  With this document expect an early boost from the content and preface pages, and then throughput plateaus out.
- Start tg-show-token-rate
- Wait for it to finish
- Record the last line produced.

## Data ingest token rates

| Platform | GPU | Model | Flow | Source material | In token/s | Out tok/s | Total tok/s |
| -------- | --- | ----- | ---- | --------------- | ---------- | ----------- | ---------- |
| VertexAI | n/a | Gemini 2.0 Flash | document-rag+graph-rag | NASA Challenger Report Volume 1 | 216.2 | 155.8 | 372.0 |
| LMStudio | Radeon RX7900 XT | Gemma2 9B | document-rag+graph-rag | NASA Challenger Report Volume 1 | 119.6 | 73.0 | 192.6 |

