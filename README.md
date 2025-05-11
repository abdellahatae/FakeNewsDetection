# FakeNewsDetection
# Kaggle Fake News Dataset (Kaggle – "Fake and real news dataset")
Lien : https://www.kaggle.com/clmentbisaillon/fake-and-real-news-dataset

Taille : ~40 000 articles

Colonnes :

-title (titre de l’article)

-text (corps complet)

-label (FAKE ou REAL)

Avantages :

-Bien structuré

-Données réelles

-Directement utilisable pour classification binaire

# Pipeline recommandé : 
## le dataset Kaggle "Fake and Real News" contient deux fichiers CSV séparés : Fake.csv et True.csv.

 -Charge les deux fichiers CSV
 
 -Fusionne les deux datasets en un seul
 
 -Nettoie les textes (title + text)
 
 -Vectorise avec TF-IDF
 
 -Entraîne un modèle SVM
 
 -Évalue le modèle
 
 -Exporte le modèle en .pkl prêt à être intégré

# Bonus : que faire ensuite ?
Le fichier fake_news_model.pkl peut ensuite être utilisé dans un microservice Python avec Flask ou FastAPI pour l’intégrer dans ton projet Spring/Angular.
