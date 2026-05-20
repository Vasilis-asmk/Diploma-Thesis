---
library_name: transformers
license: apache-2.0
base_model: facebook/hubert-base-ls960
tags:
- generated_from_trainer
datasets:
- audiofolder
metrics:
- accuracy
model-index:
- name: hubert-finetuned-CASIA
  results:
  - task:
      name: Audio Classification
      type: audio-classification
    dataset:
      name: audiofolder
      type: audiofolder
      config: default
      split: train
      args: default
    metrics:
    - name: Accuracy
      type: accuracy
      value: 0.8
---

<!-- This model card has been generated automatically according to the information the Trainer had access to. You
should probably proofread and complete it, then remove this comment. -->

# hubert-finetuned-CASIA

This model is a fine-tuned version of [facebook/hubert-base-ls960](https://huggingface.co/facebook/hubert-base-ls960) on the audiofolder dataset.
It achieves the following results on the evaluation set:
- Loss: 0.6783
- Accuracy: 0.8

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
- num_epochs: 7
- mixed_precision_training: Native AMP

### Training results

| Training Loss | Epoch | Step | Validation Loss | Accuracy |
|:-------------:|:-----:|:----:|:---------------:|:--------:|
| 6.6906        | 1.0   | 60   | 1.4090          | 0.325    |
| 5.6728        | 2.0   | 120  | 1.1344          | 0.5542   |
| 4.9187        | 3.0   | 180  | 0.9036          | 0.7042   |
| 4.3592        | 4.0   | 240  | 0.7911          | 0.75     |
| 3.4655        | 5.0   | 300  | 0.6783          | 0.8      |
| 3.1525        | 6.0   | 360  | 0.7754          | 0.7417   |
| 2.8022        | 7.0   | 420  | 0.7240          | 0.7333   |


### Framework versions

- Transformers 5.0.0
- Pytorch 2.10.0+cu128
- Datasets 4.0.0
- Tokenizers 0.22.2
