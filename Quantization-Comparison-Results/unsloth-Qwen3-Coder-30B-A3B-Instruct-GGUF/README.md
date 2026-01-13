HW: RTX 3090 24GB limited to 200W TDP

Metrics only results available as well.

Judge: gemma3-12b-it-qat + gemma3-27b-it-qat, gemma3-12b-it-qat, gemma3-27b-it-qat

Interesting takes on `Qwen3-Coder-30B-A3B-Instruct-GGUF` analysis, keep in mind is only 50 questions over 5 languages:
- `IQ3_XXS` seems to be an excellent quant, winning against the bigger `Q3_K_XL`; loses on the metrics but wins judgment both for similarity and BestAnswer
- `Q2_K_L`, `IQ4_NL` and `IQ4_XS` seems to be particularly bad; `IQ4_XS` does not work properly, some answers are garbage
- `IQ2_M` and `Q2_K_XL` are still usable despite the small size
- `Q3_K_M` seems to perform really well while being only 14,7GB
- `Q5_K_XL` and up quants are excellent except plain `Q8_0` which seems to fall a bit behind