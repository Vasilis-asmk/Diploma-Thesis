---
library_name: transformers
license: apache-2.0
base_model: facebook/hubert-base-ls960
tags:
- generated_from_trainer
metrics:
- accuracy
model-index:
- name: hubert-finetuned-ravdess
  results: []
---

<!-- This model card has been generated automatically according to the information the Trainer had access to. You
should probably proofread and complete it, then remove this comment. -->

# hubert-finetuned-ravdess

This model is a fine-tuned version of [facebook/hubert-base-ls960](https://huggingface.co/facebook/hubert-base-ls960) on an unknown dataset.
It achieves the following results on the evaluation set:
- Loss: 1.2685
- Accuracy: 0.5868

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
- train_batch_size: 8
- eval_batch_size: 8
- seed: 42
- gradient_accumulation_steps: 2
- total_train_batch_size: 16
- optimizer: Use OptimizerNames.ADAMW_TORCH_FUSED with betas=(0.9,0.999) and epsilon=1e-08 and optimizer_args=No additional optimizer arguments
- lr_scheduler_type: linear
- lr_scheduler_warmup_steps: 0.1
- num_epochs: 5
- mixed_precision_training: Native AMP

### Training results

| Training Loss | Epoch | Step | Validation Loss | Accuracy |
|:-------------:|:-----:|:----:|:---------------:|:--------:|
| 4.1153        | 1.0   | 72   | 1.8084          | 0.3264   |
| 3.7057        | 2.0   | 144  | 1.5782          | 0.3646   |
| 3.0930        | 3.0   | 216  | 1.5353          | 0.4549   |
| 2.9020        | 4.0   | 288  | 1.3189          | 0.5625   |
| 2.6149        | 5.0   | 360  | 1.2685          | 0.5868   |


### Framework versions

- Transformers 5.0.0
- Pytorch 2.10.0+cu128
- Datasets 4.0.0
- Tokenizers 0.22.2
