# Sentiment Analysis in Romanised Nepali-English Code-Switched Text
**Author:** Kshitiz Bhujel  
**Supervisor:** Dr. Bal Krishna Bal  
**Degree:** MSc in Information Technology, London Metropolitan University / Islington College  

##  Abstract
This research addresses the challenge of sentiment analysis in low-resource, code-mixed environments. [cite_start]We focus on **Romanised Nepali-English YouTube comments**, a linguistic context characterized by irregular orthography and a lack of standardized spelling[cite: 58, 103, 104]. 

[cite_start]We compared three deep learning architectures: **BiLSTM with Attention**, **mBERT**, and **XLM-ROBERTa (XLM-R)**[cite: 59]. [cite_start]Our findings demonstrate that XLM-R is the superior model for this task, though significant cross-lingual biases remain[cite: 63, 75, 76].

##  Key Findings
* [cite_start]**Model Performance:** XLM-ROBERTa achieved the highest Weighted F1-score of **75%** (compared to 71% for mBERT and 68% for BiLSTM)[cite: 757, 759].
* [cite_start]**English Bias:** Despite the multilingual nature of the models, they performed **26% better** on English text than on Romanised Nepali for the exact same sentiment[cite: 66, 67, 889].
* [cite_start]**Negation Blindness:** We identified a systematic failure where models struggle to identify Nepali negation markers like *"bhayena"* and *"naramro"*, often predicting the opposite sentiment[cite: 68, 946, 948].
* [cite_start]**Optimization:** Early stopping at **Epoch 2** is critical for preventing overfitting in these low-resource settings[cite: 62, 840, 1062].

##  Technologies Used
* [cite_start]**Languages:** Python 3.12 [cite: 624]
* [cite_start]**Frameworks:** PyTorch, Hugging Face Transformers [cite: 623]
* [cite_start]**Models:** XLM-ROBERTa-base, mBERT-base-cased, BiLSTM + Attention [cite: 133, 159, 169]

## Repository Contents
* [cite_start]`Final_dissertation_report.pdf`: The complete 15,000-word research paper[cite: 17].
* [cite_start]`Appendices/`: Includes full hyperparameter tuning results and loss curves[cite: 1250, 1277].
