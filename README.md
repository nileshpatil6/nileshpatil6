### Nilesh Patil

Software engineer — LLM/RL research, autonomous robotics, and production full-stack systems.

Merged code into the production codebases of **Apple, Microsoft, Google, OpenAI, and Hugging Face**.

**Meta × Scaler PyTorch Hackathon** Grand Finalist · **Top 30 nationally**, ISRO Robotics Challenge (IRoC-U 2026)

---

#### Merged upstream

10 pull requests merged into external projects. Each one is a defect found by reading the code, reduced to a minimal fix with a regression test.

| Org | Repo | PR | What it fixed |
|---|---|---|---|
| Apple | [ml-explore/mlx](https://github.com/ml-explore/mlx) | [#4173](https://github.com/ml-explore/mlx/pull/4173) | Python floats silently lost double precision in float64 ops — the conversion cast to float32 before the dtype was known |
| Microsoft | [microsoft/pyright](https://github.com/microsoft/pyright) | [#11620](https://github.com/microsoft/pyright/pull/11620) | Narrow closed TypedDicts on a key membership check, enabling a path the maintainer had left commented out |
| Google | [google/osv-scanner](https://github.com/google/osv-scanner) | [#2762](https://github.com/google/osv-scanner/pull/2762) | Skip malformed commit hashes instead of aborting the whole scan (+711 LOC, Go) |
| OpenAI | [openai/openai-agents-python](https://github.com/openai/openai-agents-python) | [#2931](https://github.com/openai/openai-agents-python/pull/2931) | Surface run-loop exceptions after `stream_events()` completes, instead of failing as silent truncation |
| Hugging Face | [huggingface/transformers](https://github.com/huggingface/transformers) | [#46006](https://github.com/huggingface/transformers/pull/46006) | Fix `/v1/models` response type in transformers-serve |
| Hydra | [hydra-ecosystem/hydra](https://github.com/hydra-ecosystem/hydra) | [#3365](https://github.com/hydra-ecosystem/hydra/pull/3365) | Backslashes in Defaults List paths bypassed the parent-traversal check, letting a config escape its directory |
| Hydra | [hydra-ecosystem/hydra](https://github.com/hydra-ecosystem/hydra) | [#3262](https://github.com/hydra-ecosystem/hydra/pull/3262) | Fire `on_job_end`/`on_run_end` callbacks on `KeyboardInterrupt` |
| SchemaStore | [SchemaStore/schemastore](https://github.com/SchemaStore/schemastore) | ×3 | TypeScript/JSConfig lib entries + Claude Code settings schema |

#### In review

Open pull requests at **Microsoft** (Garnet, DirectX Shader Compiler, ONNX Runtime, pyright), **NVIDIA** (Warp), **Apple** (Pkl), **Netflix** (Metaflow), **Google** (Gson), **OpenAI** (Whisper), **LinkedIn** (Liger-Kernel) and **SciPy**.

- [microsoft/garnet#2070](https://github.com/microsoft/garnet/pull/2070) — a shutdown race in the Tsavorite allocator: `Dispose()` cleared the page array before the background resizer was stopped, so a resizer still inside `EvictRecordsInRange` dereferenced it and the `NullReferenceException` was escalated to `Environment.FailFast`, killing the process.
- [NVIDIA/warp#1762](https://github.com/NVIDIA/warp/pull/1762) — tiled BVH queries silently dropped results for non-power-of-two block sizes, because the expansion step count rounded up instead of down.
- [microsoft/DirectXShaderCompiler#8782](https://github.com/microsoft/DirectXShaderCompiler/pull/8782) — the DXBC converter trusted a shader length from the container without validating it against the part size, reading out of bounds on a malformed input.

---

#### Building

- **[promptinject-env-agents](https://github.com/nileshpatil6/promptinject-env-agents)** — adversarial multi-agent RL (GRPO) for LLM prompt-injection defense; defender accuracy 47.1% → 92.8% over 30 A100 episodes. Live on Hugging Face Spaces.
- **[MindRead-RL-Environment](https://github.com/nileshpatil6/MindRead-RL-Environment)** — Theory-of-Mind RL environment, also live on HF Spaces.
- **Autonomous GNSS-denied micro-UAV** — ISRO Robotics Challenge (IRoC-U 2026), Top 30 nationally. Custom visual-inertial SLAM, ArUco precision landing, RealSense + YOLOv8 tracking on a Raspberry Pi companion computer.
- **Keepi** — local-first AI memory app on Flutter/Isar with a realtime Gemini Live voice assistant, live on Google Play.

---

[Portfolio](https://nileshpatil6.com) · [LinkedIn](https://www.linkedin.com/in/nileshpatil6) · nilesh@nileshpatil6.com
