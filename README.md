# SmolLM Learning

A hands-on course for fine-tuning, aligning, evaluating, and serving the [SmolLM2](https://huggingface.co/collections/HuggingFaceTB/smollm2-6723884218bcda64b34d7db9) family of small language models.

## Objectives

Work through the full lifecycle of adapting a small language model to a task: instruction tuning, preference alignment, parameter-efficient fine-tuning, evaluation, inference, and tracing. Each module combines conceptual guides and exercise notebooks (adapted from Hugging Face's [smol-course](https://github.com/huggingface/smol-course)) with applied SmolLM walkthrough notebooks that carry a summarization task from base model to deployment.

Supervised fine-tuning (SFT) and PEFT techniques require a task-specific dataset structured with input–output pairs; the walkthrough notebooks use a summarization task on the SmolLM2 series.

Next steps: finalize evaluation and move to the SmolLM3 series (see the HF [SmolLM3 blog post](https://huggingface.co/blog/smollm3)).

## Course Structure

| Module | Topic | Contents |
|--------|-------|----------|
| [1. Instruction Tuning](./1_instruction_tuning/README.md) | Chat templates and supervised fine-tuning | smol-course guides + `SmolLM Family`, `SmolLM text summarization` |
| [2. Preference Alignment](./2_preference_alignment/README.md) | DPO and ORPO | smol-course guides + notebooks |
| [3. PEFT](./3_peft/README.md) | LoRA, QLoRA, prompt tuning | smol-course guides + `SmolLM QLora` |
| [4. Evaluation](./4_evaluation/README.md) | Automatic benchmarks and custom domain evaluation | smol-course guides + `SmolLM Evaluation` |
| [5. Inference](./5_inference/README.md) | Text generation and generation parameters | `SmolLM Inference` |
| [6. Tracing](./6_tracing/README.md) | Experiment tracking and GPU optimization | `SmolLM Tracing` |

## Additional Notebooks

Standalone experiments on model-efficiency techniques live at the repository root:

- `gradient-checkpointing-nin.ipynb` — gradient checkpointing demo (Network-in-Network on CIFAR-10)
- `basic_pruning_mlp.ipynb`, `depth_pruning.ipynb` — pruning experiments
- `bias_compatibility_check.ipynb` — bias/compatibility checks
- `MoE 1GPU.ipynb` — mixture-of-experts on a single GPU

## Setup

Requires Python 3.12. Install dependencies with [uv](https://github.com/astral-sh/uv):

```bash
uv sync
```

or with pip:

```bash
pip install -e .
```

## Attribution

The conceptual guides and exercise notebooks in modules 1–4 are adapted from Hugging Face's [smol-course](https://github.com/huggingface/smol-course) (Apache 2.0). The `SmolLM *` walkthrough notebooks and the additional experiments are original to this repository.

## Resources for GPU Optimization

- [PyTorch GPU optimization: step-by-step guide](https://medium.com/@ishita.verma178/pytorch-gpu-optimization-step-by-step-guide-9dead5164ca2)

## Contributing

See [contribution.md](./contribution.md).
