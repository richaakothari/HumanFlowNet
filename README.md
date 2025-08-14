# HumanFlowNet

HumanFlowNet is a Natural Language Processing (NLP) pipeline designed to transform AI-generated text into content that closely resembles human-written text.  
The system analyzes linguistic and stylistic features from human-authored documents and applies them to AI-generated content, improving readability, emotional tone, and semantic flow — making the text more natural and less detectable by AI-detection tools.



🚀 Introduction
Recent advancements in AI text generation have made it easy to produce large volumes of content. However, AI-generated text often lacks the fluency, nuance, and stylistic diversity of human writing.  
**HumanFlowNet** addresses this by:
- Extracting linguistic features from human-written samples.
- Modifying AI-generated text using advanced NLP techniques.
- Enhancing readability, lexical diversity, and emotional tone.
- Reducing detectability by AI-authorship detection tools.



✨ Features
- **Feature Extraction:** Readability scores, lexical density, sentence variation, punctuation density, repetition ratio, sentiment analysis, and semantic coherence.
- **Text Transformation:** Uses transformer-based paraphrasing and synonym substitution strategies.
- **Similarity Scoring:** TF-IDF cosine similarity & sentence embedding similarity.
- **Classification:** Predicts if text is AI or human-written using Random Forest, SVM, and Logistic Regression.
- **Visualization:** Bar charts, radar charts, readability flow graphs, and classifier probability plots.



## 🛠 System Architecture
1. **Input Stage:** Accepts PDF documents containing AI-generated or human-authored text.
2. **Text Extraction:** Uses `PyPDF2` for reading and converting PDFs to text.
3. **Preprocessing:** Tokenization, stopword removal, and chunking.
4. **Feature Engineering:** Extraction of multiple linguistic and semantic metrics.
5. **Text Modification:** Adaptive transformations using T5 paraphraser and WordNet synonyms.
6. **Similarity Computation:** Compares modified AI text with human text samples.
7. **Visualization:** Displays feature comparisons and classifier probabilities.


## 💻 Tech Stack
- **Language:** Python 3.x  
- **Libraries & Frameworks:**
  - NLP: `nltk`, `textstat`, `transformers`, `sentence-transformers`
  - ML: `scikit-learn`
  - Visualization: `matplotlib`, `seaborn`
  - PDF Handling: `PyPDF2`, `ReportLab`
- **Models:** Sentence-BERT, T5 Paraphraser, VADER Sentiment Analyzer


## 📦 Installation
```bash
# Clone this repository
git clone https://github.com/richaakothari/HumanFlowNet.git

# Navigate to the project folder
cd HumanFlowNet

# Install dependencies
pip install -r requirements.txt
