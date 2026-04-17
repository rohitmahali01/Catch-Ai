
# Catch AI: Fine-Grained Human-AI Collaborative Text Detection

### 🚀 A Dual-Branch Semantic-Stylometric Approach
**Author:** Rohit Mahali (22190503048)  
**Institution:** Central University of Jharkhand, Ranchi  
**Guides:** Prof. Subhash Chandra Yadav & Dr. Dali Ramu Burada  

---

## 📌 Overview
`Catch AI` is a research prototype designed to distinguish between human-written, AI-generated, and **hybrid (co-authored)** text. 

Current Transformer-based detectors (like RoBERTa) are often fooled by **adversarial attacks** such as:
1. **Topic Masking:** Using rare/technical vocabulary.
2. **Style Transfer:** Using casual slang or informal tones.
3. **Academic Mimicry:** Using formal transitional phrases.

This project implements a **Dual-Branch Architecture** to overcome these vulnerabilities.

## 🛠️ Methodology: The Dual-Branch System
This system analyzes text through two concurrent lenses:

1. **Semantic Branch (Deep Learning):** Utilizes a fine-tuned **RoBERTa-base** model to analyze contextual meaning and document-level patterns.
2. **Stylometric Branch (Structural Novelty):** Analyzes the "mathematical rhythm" of writing.
   - **Burstiness (Perplexity Variance):** Measures the standard deviation of sentence lengths. Humans write with high variance; AI writes with robotic uniformity.
   - **Syntactic Fingerprinting:** Extracts Part-of-Speech (POS) ratios (Nouns/Verbs/Adjectives) to detect synthetic grammatical patterns.

## 📊 Key Features
- **Sentence-Level Heatmaps:** Visualizes the transition points between human and AI text.
- **Stylometric Radar Charts:** Maps the linguistic "fingerprint" of the input text.
- **Burstiness Scoring:** Provides a stable, vocabulary-independent signal of authorship.

## 💻 Installation & Usage

### Prerequisites
- Python 3.8+
- PyTorch

### Setup
1. Clone the repository:
   ```bash
   git clone https://github.com/your-username/catch-ai.git
   cd catch-ai
   ```

2. Install dependencies:
   ```bash
   pip install -r requirements.txt
   python -m spacy download en_core_web_sm
   ```

3. Run the application:
   ```bash
   streamlit run app.py
   ```

## 📖 Research Foundations
This project is an extension of and inspired by the following research:
- **Lekkala et al. (2025):** Fine-Grained Detection via Sentence-Level Segmentation.
- **Aityan et al. (2025):** Lightweight Stylometric Feature Detection.
- **Su et al. (2025):** Human-AI Coauthoring (HACo-Det).
- **He et al. (2025):** DETree framework for model attribution.

---
© 2026 Rohit Mahali | Bachelor of Engineering in Computer Science and Engineering
```
