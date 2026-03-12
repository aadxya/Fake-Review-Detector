# Fake Review Detector (NLP + Streamlit)

A machine learning project that detects **fake vs real** product reviews using **TF-IDF vectorization**, **Logistic Regression**, and **behavioral text features** such as exclamation count, sentiment, and repeated promotional phrases.  

---

## Features
- Text cleaning and normalization pipeline  
- Hybrid feature extraction:
  - TF-IDF (1–2 grams)
  - Numeric sentiment & behavioral features  
- Interpretable Logistic Regression model  
- Evaluation metrics: Confusion Matrix, ROC, and PR curves  
- Interactive Streamlit app with adjustable decision threshold  

---



---

## How It Works

1. **Data Input:** CSV containing `text` and `label` columns.  
2. **Preprocessing:** URL, punctuation, and HTML removal + lowercasing.  
3. **Feature Engineering:**  
   - Sentiment score  
   - Exclamation & ALL-CAPS detection  
   - Fake-review clichés (e.g., “best product ever”)  
4. **Modeling:** Logistic Regression trained on combined features.  
5. **Prediction:** Threshold-tunable classification for FAKE vs REAL.  

---

## Insights
- Excessive punctuation, emotional exaggeration, or ALL-CAPS usage strongly correlates with fake reviews.  
- Real reviews tend to include neutral tone and product-specific feedback.  
- The combination of linguistic + behavioral features improves reliability over text-only models.

---

## Future Improvements
- Integrate a larger, real-world labeled dataset.  
- Replace TF-IDF with contextual embeddings (BERT/SentenceTransformer).  
- Deploy via Streamlit Cloud or Hugging Face Spaces.  
- Add explainability (SHAP/LIME) for feature-level insights.
