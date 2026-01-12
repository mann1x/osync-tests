# [osync](https://github.com/mann1x/osync) - test results

Repository for my tests with osync
Currently only *Quantizations Comparisons*

Testing HW: RTX3090 TDP limited to 200W

As for the best `ollama` model as Judge my pick is currently `gemma-3`:
- the `12b` is very good at similarity score but when judging which answer is the best seems to be biased toward the response from the quantized model.
- the `27b` is NOT very good at similarity score but when judging which answer is the best is definitely more accurate.

I will implement next an optional split to use different judge models for similarity and best answer.

Models tested so far:

- [unsloth/Qwen3-Coder-30B-A3B-Instruct-GGUF](https://huggingface.co/unsloth/Qwen3-Coder-30B-A3B-Instruct-GGUF)
  - Judge: gemma3-12b [Quantization-Comparison-Results/unsloth-Qwen3-Coder-30B-A3B-Instruct-GGUF](https://github.com/mann1x/osync-tests/tree/main/Quantization-Comparison-Results/unsloth-Qwen3-Coder-30B-A3B-Instruct-GGUF)
    - [View Benchmark Report (HTML)](https://mann1x.github.io/osync-tests/Quantization-Comparison-Results/unsloth-Qwen3-Coder-30B-A3B-Instruct-GGUF/unsloth-Qwen3-Coder-30B-A3B-Instruct-GGUF-v1code-gemma3-12b.qc.html)
    - [View Benchmark Report (PDF)](https://mann1x.github.io/osync-tests/Quantization-Comparison-Results/unsloth-Qwen3-Coder-30B-A3B-Instruct-GGUF/unsloth-Qwen3-Coder-30B-A3B-Instruct-GGUF-v1code-gemma3-12b.qc.pdf)
  - Judge: gemma3-27b [Quantization-Comparison-Results/unsloth-Qwen3-Coder-30B-A3B-Instruct-GGUF](https://github.com/mann1x/osync-tests/tree/main/Quantization-Comparison-Results/unsloth-Qwen3-Coder-30B-A3B-Instruct-GGUF)
    - [View Benchmark Report (HTML)](https://mann1x.github.io/osync-tests/Quantization-Comparison-Results/unsloth-Qwen3-Coder-30B-A3B-Instruct-GGUF/unsloth-Qwen3-Coder-30B-A3B-Instruct-GGUF-v1code-gemma3-27b.qc.html)
    - [View Benchmark Report (PDF)](https://mann1x.github.io/osync-tests/Quantization-Comparison-Results/unsloth-Qwen3-Coder-30B-A3B-Instruct-GGUF/unsloth-Qwen3-Coder-30B-A3B-Instruct-GGUF-v1code-gemma3-27b.qc.pdf)


## Examples of console output


With Judge results:

![Judge results](https://github.com/mann1x/osync-tests/blob/main/osync-console-output-judge-example.png?raw=true)


Only metrics:

![Judge results](https://github.com/mann1x/osync-tests/blob/main/osync-console-output-metrics-example.png?raw=true)
