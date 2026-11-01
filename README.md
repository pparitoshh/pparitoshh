# Hi, I am Paritosh Gupta

Data scientist at HelloFresh in Berlin. I work on search and ranking, recommender systems and LLMs.
I build small open models and tools for AI agents that run on a laptop or a CPU.

## Open models on Hugging Face

| Model | What it does | Start |
|---|---|---|
| [SlurmPilot-4B-GGUF](https://huggingface.co/gparitosh007/SlurmPilot-4B-GGUF) | A 2.5 GB local agent for Slurm and HPC clusters. It reads `squeue`, `sacct` and job logs through 17 MCP tools, and then answers. | `ollama run hf.co/gparitosh007/SlurmPilot-4B-GGUF:Q4_K_M` |
| [Open-Decision-Model-150M](https://huggingface.co/gparitosh007/Open-Decision-Model-150M) | A decision model of the Jev / Laya type. It returns a calibrated probability for each option, for LLM routing and tool-risk checks. 52 ms on a CPU. Apache 2.0. | Free MCP: `https://decision-model.vercel.app/mcp` |
| [Open-Decision-Model-150M-ONNX](https://huggingface.co/gparitosh007/Open-Decision-Model-150M-ONNX) | The fp16 ONNX export of the decision model. Runs without PyTorch. | `model_fp16.onnx` |

Add the decision model to Claude Code:

```bash
claude mcp add --transport http decision https://decision-model.vercel.app/mcp
```

## Projects

| Project | What it does |
|---|---|
| [alembic](https://github.com/pparitoshh/alembic) | DistillKit: teacher-student distillation for local HPC assistants. The harness for SlurmPilot-4B. |
| [fitcheck](https://github.com/pparitoshh/fitcheck) | Measured GPU, memory, time and cost estimates for fine-tuning small LLMs on HPC clusters, with uv and Slurm setups. |
| [driftguard](https://github.com/pparitoshh/driftguard) | A Claude Code plugin that reviews a branch against its plan, the Claude session and the git history. Local and free. |
| [ds-ml-bench](https://github.com/pparitoshh/ds-ml-bench) | A personal benchmark of LLMs on real data science and ML tasks. |
| [ai-job-search](https://github.com/pparitoshh/ai-job-search) | A job application framework on Claude Code: job evaluation, tailored CVs and interview preparation. |
| [ai-engineering-notes](https://github.com/pparitoshh/ai-engineering-notes) | Open notes on LLMs, evaluation, agentic AI, RAG and fine-tuning. |

## Highlights

- Team Alembic, EuroHPC AI Factories hackathon, October 2026. We distilled Qwen3-235B into a 4B Slurm assistant on B300 GPUs.

## Contact

[LinkedIn](https://www.linkedin.com/in/paritosh-gupta-3aa79931/) · [Hugging Face](https://huggingface.co/gparitosh007)
