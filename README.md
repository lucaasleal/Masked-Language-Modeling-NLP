# Masked-Language-Modeling-NLP

This is a deep learning project that explores the internal mechanics of Transformer-based models.  
It demonstrates masked word prediction using BERT and visualizes multi-head self-attention through attention heatmaps.

This project helps understand how Transformers distribute contextual focus across tokens in a sentence.

---

## 🚀 Features

- 🔍 Masked word prediction using `bert-base-uncased`
- 🧠 Extraction of attention weights from every layer and head
- 🎨 Automatic generation of attention heatmaps (PNG images)
- 📊 Visualization of token-to-token attention relationships
- ⚡ Built with TensorFlow and HuggingFace Transformers

---

## 📝 Example

Example input sentence:
> Artificial intelligence is transforming the future of [MASK].


Example predictions:
> Artificial intelligence is transforming the future of society.  
> Artificial intelligence is transforming the future of humanity.  
> Artificial intelligence is transforming the future of technology.

The _generate_diagram_ generating a image from each layer and head.
Each image represents the attention matrix of one head in one layer.

- Brighter cells → Higher attention weight  
- Darker cells → Lower attention weight

Example (Layer 3 and Head 7):

<img width="640" height="640" alt="Attention_Layer3_Head7" src="https://github.com/user-attachments/assets/3d027e42-4757-43cb-9fb7-2e34ec1282ff" />
---

## 🧠 Concepts Demonstrated

- Transformer Architecture
- Self-Attention Mechanism
- Multi-Head Attention
- Masked Language Modeling (MLM)
- Attention Matrix Visualization
- Contextual Word Representations
- Deep Learning for NLP

---
## 📦 Installation
Clone this repo and run project:
```bash
git clone https://github.com/lucaasleal/Masked-Language-Modeling-NLP.git
cd Masked-Language-Modeling-NLP
python mask.py
```

Enter a sentence containing the [MASK] token when prompted.
The program will:
- Predict the top K masked word candidates
- Extract attention weights
- Generate attention heatmaps for each layer and head

---
## 🔬 Model Used

- bert-base-uncased
- Framework: TensorFlow
- Library: HuggingFace Transformers

---
## 📚 References
Devlin et al., "BERT: Pre-training of Deep Bidirectional Transformers for Language Understanding"   
HuggingFace Transformers Documentation

## 👤 Author
@lucaasleal
