---
library_name: transformers
license: apache-2.0
base_model: facebook/hubert-base-ls960
tags:
- generated_from_trainer
metrics:
- accuracy
model-index:
- name: hubert-finetuned-IEMOCAP
  results: []
---

<!-- This model card has been generated automatically according to the information the Trainer had access to. You
should probably proofread and complete it, then remove this comment. -->

# hubert-finetuned-IEMOCAP

This model is a fine-tuned version of [facebook/hubert-base-ls960](https://huggingface.co/facebook/hubert-base-ls960) on an unknown dataset.
It achieves the following results on the evaluation set:
- Loss: 1.5513
- Accuracy: 0.4039

## Model description

More information needed

## Intended uses & limitations

More information needed

## Training and evaluation data

More information needed

## Training procedure

### Training hyperparameters

The following hyperparameters were used during training:
- learning_rate: 3e-05
- train_batch_size: 4
- eval_batch_size: 8
- seed: 42
- gradient_accumulation_steps: 4
- total_train_batch_size: 16
- optimizer: Use OptimizerNames.ADAMW_TORCH_FUSED with betas=(0.9,0.999) and epsilon=1e-08 and optimizer_args=No additional optimizer arguments
- lr_scheduler_type: linear
- lr_scheduler_warmup_steps: 0.1
- num_epochs: 5
- mixed_precision_training: Native AMP

### Training results

| Training Loss | Epoch | Step | Validation Loss | Accuracy |
|:-------------:|:-----:|:----:|:---------------:|:--------:|
| 6.7943        | 1.0   | 402  | 1.6983          | 0.3286   |
| 6.4488        | 2.0   | 804  | 1.6299          | 0.3472   |
| 6.4305        | 3.0   | 1206 | 1.6085          | 0.3510   |
| 6.0358        | 4.0   | 1608 | 1.5685          | 0.3945   |
| 5.7933        | 5.0   | 2010 | 1.5513          | 0.4039   |


### Framework versions

- Transformers 5.0.0
- Pytorch 2.10.0+cu128
- Datasets 4.0.0
- Tokenizers 0.22.2
