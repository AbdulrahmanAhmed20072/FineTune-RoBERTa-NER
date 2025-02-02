# Fine-Tuning RoBERTa for Named Entity Recognition (NER)

This repository fine-tunes RoBERTa for Named Entity Recognition (NER) using Parameter-Efficient Fine-Tuning (PEFT) with LoRA and BitsAndBytes quantization.

## Features

- **RoBERTa Fine-Tuning**: Adapts RoBERTa for token classification (NER).
- **LoRA & BitsAndBytes**: Efficient training with low-rank adaptation and 8-bit quantization.
- **Dataset Preparation**: Uses the CoNLL-2003 dataset for training.
- **Training Pipeline**: Utilizes Hugging Face `Trainer` for efficient model training.
- **Evaluation**: Computes precision, recall, F1-score, and accuracy using `seqeval`.

## Files

1. **`TokenClassification_RoBERTa.ipynb`**: Python script implementing the training pipeline.
2. **Dataset**: CoNLL-2003 dataset for Named Entity Recognition.

## Installation

1. Clone the repository:
   ```bash
   git clone https://github.com/AbdulrahmanAhmed20072/FineTune-RoBERTa-NER.git
   ```
2. Install the required dependencies:
   ```bash
   pip install datasets bitsandbytes evaluate seqeval peft torch transformers
   ```

## Usage

1. Load and preprocess the dataset.
2. Fine-tune RoBERTa with LoRA and quantization.
3. Evaluate model performance.
4. Predict NER tags for new sentences.

Run the script:
```bash
python TokenClassification_RoBERTa.ipynb
```

## Outputs

- Fine-tuned RoBERTa model for Named Entity Recognition.
- Precision, recall, and F1-score evaluation on test data.
- Named entity predictions for input sentences.

## Example

Input Sentence:
```
Mike goes to his grandma everyday.
```

Predicted Tags:
```
PER O O O O O
```
