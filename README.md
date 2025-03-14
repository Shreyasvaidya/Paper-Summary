# Paper-Summary
A repository for organizing summaries of papers I read. Mostly around Domain adaptation, Vision Language Models for Open Vocabulary Object Detection and LLM finetuning. 

## Domain Adaptation papers
1) Domain-Adversarial Training of Neural Networks
 
   [Summary](Domain%20Adaptation%20Papers/Domain-Adversarial%20Training%20of%20Neural%20Networks/Readme.md)   [Paper Link](https://jmlr.org/papers/volume17/15-239/15-239.pdf)

   This work intends to peform classification tasks using representations which are indistinguishable between the source and target domains by a trained domain classifier

## Vision Language Models for Object Detection
1) Grounded Language-Image Pre-training
 
   [Summary](VLM4OVOD/GLIP/Readme.md) [Paper Link](https://openaccess.thecvf.com/content/CVPR2022/papers/Li_Grounded_Language-Image_Pre-Training_CVPR_2022_paper.pdf)
  
   Object detection is the task of detecting objects given a few target classes. Phrase grounding is the task of finding regions in image which align with each word in a given    phrase. This paper unifies the two tasks by either giving phrases (for phrase grounding) or target classes (for object detection) as text input to the model.
 
## LLM finetuning papers
1) QLORA: Efficient Finetuning of Quantized LLMs

   [Summary](LlmFinetuning/QLora/Readme.md) [Paper Link](https://openreview.net/pdf?id=OUIFPHEgJU)

   They introduce several optimizations such as double quantization, paged optimizers as well a 4 bit NormalFloat datatype which make finetuning a mid-sized 65B parameter       model possible on a single 48 GB GPU.

