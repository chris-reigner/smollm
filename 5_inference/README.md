# Inference

Once a model has been fine-tuned, evaluated, and validated, the final step is running inference — generating outputs for real inputs, efficiently and reproducibly. This module covers how to load SmolLM2 models and generate text, along with the parameters that control generation quality and speed.

## Contents

Key topics for running inference with small language models:

- **Loading models** — loading base and fine-tuned SmolLM2 checkpoints with `transformers`.
- **Generation parameters** — controlling output with `temperature`, `top_p`, `top_k`, `max_new_tokens`, and sampling vs. greedy decoding.
- **Chat inference** — applying chat templates for instruction-tuned models.
- **Efficiency** — batching, quantization, and device placement for inference on constrained hardware.

## SmolLM Walkthrough Notebooks

| Notebook | Description |
|----------|-------------|
| [5. SmolLM Inference](./5.%20SmolLM%20Inference.ipynb) | Load a SmolLM2 model and run text generation, walking through the main generation parameters |

## Resources

- [Transformers generation strategies](https://huggingface.co/docs/transformers/main/en/generation_strategies)
- [Text generation with `transformers`](https://huggingface.co/docs/transformers/main/en/llm_tutorial)
- [SmolLM2 model collection](https://huggingface.co/collections/HuggingFaceTB/smollm2-6723884218bcda64b34d7db9)
