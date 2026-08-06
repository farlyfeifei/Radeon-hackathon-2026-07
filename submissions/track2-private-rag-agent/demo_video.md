# Demo Video

**Private RAG Agent — Track 2 (2026 AMD AI DevMaster Hackathon)**

## 🎬 Primary video (submitted)

**`private_rag_agent_demo.mp4`** (in this folder) — 3 min 26 s, 1280×800, H.264.
A screen capture of the actual application running end to end:

1. **Opening** — the empty-state UI: "100% local, offline, data never leaves this machine".
2. **Document ingestion** — the knowledge base shows 6 documents · 15 chunks.
3. **Single-agent Q&A** — live tool-call trace, streaming answer, citation cards.
4. **Multi-agent parallel** — plan panel with 3 sub-tasks and progress bar, three parallel
   researcher agents, fact-check cards with grounding scores, and the synthesized answer
   with a per-sentence verification panel.
5. **GPU acceleration** — the in-app GPU monitor.
6. **Source drawer** — clicking a citation opens the original document.

> The video is silent; a narrated version with the full shot-by-shot script
> (`src/docs/demo_video_EN.md`) can be recorded if desired. Video link for hosting:
> _(add Bilibili / YouTube URL here after upload)_

---

## What the video demonstrates

1. **Opening** — the empty-state UI: "100% local, offline, data never leaves this machine".
2. **Document ingestion** — importing PDF/Word/Markdown into the local knowledge base; badge updates to *6 documents · 15 chunks*.
3. **Single-agent Q&A** — live tool-call trace (`rag_search`), streaming answer, clickable citation cards, and the source drawer with query terms highlighted in the original text.
4. **Multi-agent parallel** (the climax) — the plan panel with 3 sub-tasks and a progress bar, three parallel researcher agents streaming retrieval events, fact-check cards with grounding scores, and the final answer composed only from verified content.
5. **GPU acceleration** — the in-app GPU monitor (utilization / VRAM / temperature) plus `rocm-smi` / `benchmarks/bench_amd.py` evidence from the AMD Radeon (ROCm) environment.
6. **Closing** — "retrieval you can trace, answers you can verify, data that stays on this machine."

---

## Narration script

The full shot-by-shot English narration and production notes are in
[`src/docs/demo_video_EN.md`](src/docs/demo_video_EN.md) (also available as
[`demo_video_script.pdf`](demo_video_script.pdf)).

## Recording notes

- Record with OBS Studio / Bandicam: 1920×1080, 60 fps, high bitrate, MP4/H.264.
- All functional shots (1–4) run fully live on a CPU-only machine — no GPU required.
- The GPU shot uses real `rocm-smi` output and `bench_amd.py` measurements from the Radeon Cloud instance; demo numbers are never faked.
