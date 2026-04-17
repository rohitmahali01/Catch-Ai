### **1. Repository Structure**
```text
catch-ai/
├── app.py              # The main Streamlit application code
├── requirements.txt    # Python dependencies
├── README.md           # Project documentation (The most important file)
├── .gitignore          # Files to ignore (like __pycache__)
├── assets/             # Folder for screenshots of your Heatmaps/Radar charts
└── research/           # Your Dissertation Abstract and PDF report
```

---

### **2. The `README.md` Content**
Copy and paste this into your `README.md` file. It explains your "Dual-Branch" methodology to anyone who visits the page.

```markdown
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

---

### **3. The `requirements.txt` Content**
Create a file named `requirements.txt` and paste these libraries:

```text
streamlit
torch
transformers
numpy
plotly
spacy
nltk
```

---

### **4. The `.gitignore` Content**
This keeps your repo clean from temporary files:

```text
__pycache__/
.streamlit/
*.pyc
.env
```

---

### **How to "Commit" this to GitHub:**

1. **Create the Repo:** Go to GitHub and create a new repository named `catch-ai`.
2. **Initialize locally:**
   ```bash
   git init
   git add .
   git commit -m "Initial commit: Dual-branch hybrid AI detection prototype"
   ```
3. **Push to GitHub:**
   ```bash
   git remote add origin https://github.com/your-username/catch-ai.git
   git branch -M main
   git push -u origin main
   ```

### **💡 Final Tip for your Presentation:**
During your demo, open your GitHub repo and show the professors your **README**. It proves that your work is professionally documented and that you are following **Open Science** practices by sharing your code and research foundations.
