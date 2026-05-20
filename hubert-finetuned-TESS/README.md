---
library_name: transformers
license: apache-2.0
base_model: facebook/hubert-base-ls960
tags:
- generated_from_trainer
metrics:
- accuracy
model-index:
- name: hubert-finetuned-TESS
  results: []
---

<!-- This model card has been generated automatically according to the information the Trainer had access to. You
should probably proofread and complete it, then remove this comment. -->

# hubert-finetuned-TESS

This model is a fine-tuned version of [facebook/hubert-base-ls960](https://huggingface.co/facebook/hubert-base-ls960) on an unknown dataset.
It achieves the following results on the evaluation set:
- Loss: 0.2848
- Accuracy: 1.0

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
| 9.1729        | 1.0   | 140  | 1.3954          | 0.95     |
| 4.3874        | 2.0   | 280  | 0.5802          | 0.9982   |
| 2.1819        | 3.0   | 420  | 0.2848          | 1.0      |
| 1.2389        | 4.0   | 560  | 0.1720          | 1.0      |
| 1.1367        | 5.0   | 700  | 0.1435          | 1.0      |


### Framework versions

- Transformers 5.0.0
- Pytorch 2.10.0+cu128
- Datasets 4.0.0
- Tokenizers 0.22.2
