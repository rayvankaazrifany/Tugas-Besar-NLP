| Nama | NIM |
|------|-----|
| Mochamad Rafly Taufik Putra Fadilah | 10522022 |
| Aydil Harsy Putra | 10522021 |
| Rayvanka Azrifany Nurviana Najmi | 10522010 |
| Niken Nuraifah Suherlan | 10522018 |

Program Studi Sistem Informasi, Universitas Komputer Indonesia (UNIKOM), Bandung.

## Deskripsi File Colab dan Dataset

Dataset Raw: google_reviews_richeese_pizza.xlsx
1. Data Cleaning:
        Colab: NLP_PreprocessingforRoBERTa.ipynb 
        Dataset Hasil Cleaning: dataset_pizza_cleaned.xlsx
2. labelling Sentimen degan RoBERTa Sentiment Classifier:
        Colab: NLP_SentimentClassificationRoBERTa.ipynb
        Dataset Hasil Labelling Sentimen: dataset_pizza_sentiment.xlsx
3. Pre-processing for Aspect Labelling:
        Colab: NLP_PreprocessingforAspect.ipynb
        Dataset Hasil Pre-processing: preprocessed_pizza.xlsx
4. Aspect Labelling:
        Aspect Dictionary: aspect_dictionary_pizza.json
        Colab: NLP_AspectLabelling.ipynb
        Dataset Hasil Aspect Labelling: sentiment_aspect_analysis.xlsx
5. Modelling:
        Colab: NLP_ModellingIndoBERT_absa_richeese.ipynb


## Hasil Ringkas

**Dataset:** 3.291 ulasan mentah → 2.012 data bersih setelah cleaning.

**Distribusi Sentimen:** Positif 85,8% | Negatif 12,4% | Netral 1,8%

**Distribusi Aspek:** Makanan 34,0% | Suasana 25,7% | Pelayanan 25,3% | Fasilitas 9,6% | Harga 5,3%

**Model Sentimen (single-label, 3 kelas):**
- Akurasi: 93,07%
- Macro F1-score: 80,80%

**Model Aspek (multi-label, 5 kelas):**
- Macro F1-score: 90,63%
- Micro F1-score: 91,95%
- Hamming Loss: 0,0693
- F1-score tertinggi: aspek pelayanan (96,52%)
- F1-score terendah: aspek fasilitas (78,65%)
