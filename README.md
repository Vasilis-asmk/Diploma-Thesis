Speech Emotion Recognition with Transformer Models (Ανάλυση Συναισθηματικής Κατάστασης από Ομιλία με χρήση Transformer)

Code for Diploma Thesis: Speech Emotion Recognition with Transformer Models. In this thesis 
transformer models (data2vec, HuBERT, wav2vec 2.0, WavLM, UniSpeech-SAT, Whisper, AST and wav2vec-conformer) are 
finetuned for speech emotion recognition (SER) on appropriate datasets (TESS, CREMA-D, RAVDESS, IEMOCAP, SAVEE 
and ESD) and are then analyzed through explainability (XAI), embedding space and cross-corpus evaluation.

This repository contains code only, finetuned model are stored on the equivalent checkpoint on the Hugging Face Hub, based on the table below.

##Models and datasets

| Model | Dataset | Finetuned model repo |
| data2vec | TESS | VasilisAsim/data2vec-finetuned-TESS_full |
| hubert | RAVDESS | VasilisAsim/hubert-finetuned-Ravdess | 
| data2vec | CREMA-D | VasilisAsim/data2vec-finetuned-CREMA-D |
|data2vec | RAVDESS | VasilisAsim/data2vec-finetuned-ravdess |
|data2vec | IEMOCAP | VasilisAsim/data2vec-finetuned-IEMOCAP-categorical |
|wav2vec | TESS | VasilisAsim/wav2vec-finetuned-TESS |
|UniSpeech-SAT | IEMOCAP | VasilisAsim/unispeech_sat-finetuned-IEMOCAP
|HuBERT | SAVEE | VasilisAsim/hubert-finetuned-SAVEE |
|Whisper | TESS | VasilisAsim/whisper-finetuned-TESS | 
| AST | RAVDESS | VasilisAsim/AST-finetuned-ravdess |
|Whisper | RAVDESS | VasilisAsim/whisper-finetuned-Ravdess |
|WavLM | CREMA-D | VasilisAsim/wavlm-finetuned-cremad |
|wav2vec-conformer | CREMA-D | VasilisAsim/wav2vec2-conformer-finetuned-CREMA-D |
|wav2vec | IEMOCAP | VasilisAsim/wav2vec-finetuned-iemocap |	
| data2vec | SAVEE | VasilisAsim/data2vec-finetuned-SAVEE |
|Whisper | SAVEE | VasilisAsim/whisper-finetuned-SAVEE | 
|WavLM | IEMOCAP | VasilisAsim/wavlm-finetuned-IEMOCAP |
| AST | TESS | VasilisAsim/ast-finetuned-TESS |
| AST | CREMA-D | VasilisAsim/AST-finetuned-CREMA_D |
| HuBERT | CREMA-D | VasilisAsim/hubert-finetuned-CREMA-D |
| UniSpeech-SAT | CREMA-D | VasilisAsim/unispeech-sat-finetuned-ESD |
| UniSpeech-SAT | ESD | VasilisAsim/Unispeech_SAT_fnetuned_esd_english |
| wav2vec | ESD | VasilisAsim/wav2vec2-finetuned-ESD |
| WavLM | ESD | VasilisAsim/wavlm-finetuned-ESD |
