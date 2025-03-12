
# QLORA: Efficient Finetuning of Quantized LLMs
# NeurIPS ‘23
[Paper Link](https://openreview.net/pdf?id=OUIFPHEgJU)
Fine-tuning Large language models is the standard way to adapt them to new tasks. But full finetuning is memory-expensive. A mid-sized 65B model with 16 bit floating point weights requires greater than 780 GB memory (and even training Low Rank adapters [1] requires around 150 GB memory according to this specification). 
This paper introduces several optimisations which make it possible to finetune models with much lesser memory without drop in performance. A 65-B Llama can be finetuned using QLoRA on a single 48 GB GPU. 
The paper uses several optimizations as well as introduces several new ones such as 4 bit NormalFloat datatype, double quantization and paged optimizers to make model finetuning efficient without loss in performance.
## Background
### Low Rank adaptation
In Low Rank adaptation (LoRA finetuning), the weight updates 〖∆W〗_(d*d) are represented as a product of 2 matrices A_(d*r) and B_(r*d). These matrices are of much lower rank  as compared to W (d≪r) and hence can be tuned much more efficiently, but still have shown to give performance improvements comparable to full finetuning.
