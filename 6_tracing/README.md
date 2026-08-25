# Tracing & Monitoring

Training and fine-tuning are far easier to debug and optimize when you can see what's happening. Tracing captures metrics, hyperparameters, and system stats (GPU utilization, memory, throughput) so you can compare runs, catch regressions, and push hardware to its limits. This module uses [Weights & Biases](https://wandb.ai) to instrument a SmolLM2 fine-tuning run.

## Contents

- **Experiment tracking** — logging loss, learning rate, and custom metrics with `wandb` and the Hugging Face `Trainer` integration.
- **System monitoring** — tracking GPU utilization and memory to find bottlenecks.
- **GPU optimization** — using traces to drive GPU consumption toward its capacity.

## SmolLM Walkthrough Notebooks

| Notebook | Description |
|----------|-------------|
| [6. SmolLM Tracing](./6.%20SmolLM%20Tracing.ipynb) | Instrument a SmolLM2 fine-tuning run with Weights & Biases and monitor/optimize GPU consumption |

## Resources

- [W&B Hugging Face integration](https://docs.wandb.ai/guides/integrations/huggingface/)
- [Weights & Biases documentation](https://docs.wandb.ai)
