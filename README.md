# Text-Style-Transfer-using-NLP-techniques
This project implements and evaluates various Natural Language Processing (NLP) approaches to **text style transfer**—converting text from one style to another (e.g., informal → formal)—while preserving the original content.

## 🧠 Project Overview

The main objective is to compare how different models perform in transforming text style without losing meaning. This includes:

- **Seq2Seq (LSTM-based encoder-decoder)**
- **T5 (Text-to-Text Transformer)**
- **GPT-2 fine-tuned for style transfer**
- Possibly leveraging a **Hugging Face pre-trained model** as a baseline

## 📋 Dataset

- Likely used: **GYAFC (Grammarly’s Yahoo Answers Formality Corpus)** or similar parallel dataset.
- Covers domains such as *Entertainment & Music* and *Family & Relationships*.
- Contains paired informal ↔ formal sentences.

*(Update this section with the actual dataset name, source link, and preprocessing steps.)*

## 🛠 Installation & Setup

1. **Clone the repository**  
   ```bash
   git clone https://github.com/dheerajraqesh/Text-Style-Transfer-using-NLP-techniques.git
   cd Text-Style-Transfer-using-NLP-techniques
Install dependencies
pip install -r requirements.txt
Download the dataset (if not included) and place it in the project folder (e.g., data/).
Train or fine-tune models by running scripts such as:
python train_t5.py
python train_gpt2.py
Generate style transfer output:
python inference.py --input "your informal sentence here"
🚀 Workflow & Components

Data Preprocessing: Cleansing, tokenization, encoding categorical features if any.
Model Training/Fine-tuning:
Seq2Seq LSTM model
Pretrained T5 and GPT-2 models fine-tuned on style transfer dataset
Baseline Models:
Hugging Face pre-trained style-transfer models 
Inference: Apply trained models to convert input text and visualize results.
📊 Evaluation

Performance is measured using:

BLEU score for style accuracy
TER (Translation Edit Rate) for edit sparsity
Human evaluation or qualitative assessment on fluency and style adherence
