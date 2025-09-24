# -
#  NLP Ανακατασκευή και Σημασιολογική Ανάλυση Κειμένων

Αυτό το αποθετήριο περιέχει την υλοποίηση των Παραδοτέων 1, 2 και 3 της εργασίας με θέμα τη σημασιολογική ανακατασκευή, ενσωματώσεις λέξεων και σύγκριση τεχνικών NLP.

---

##  Δομή Φακέλων

```
├── notebooks/             # Jupyter Notebooks με ανάλυση και πειραματισμούς
├── scripts/               # Python scripts για pipelines ανακατασκευής
├── results/               # Ανακατασκευασμένα κείμενα (.txt/.json)
├── visualizations/        # Γραφικές αναπαραστάσεις PCA/t-SNE, heatmaps
├── data/                  # Αρχικά κείμενα και embeddings (αν χρειάζεται)
├── models/                # Αποθηκευμένα μοντέλα (αν εφαρμοστεί)
├── .env                   # Περιέχει κλειδιά API (excluded)
├── .gitignore             # Αποκλείει αρχεία .env, model weights κλπ.
└── README.md              # Αυτή η περιγραφή του project
```

---

##  Παραδοτέο 1 – Ανακατασκευή Κειμένων

- **A. Custom αυτόματη ανακατασκευή 2 προτάσεων**
- **B. Ανακατασκευή με 3 διαφορετικά μοντέλα (BART, T5, Pegasus)**
- **Γ. Σύγκριση ποιότητας με cosine similarity, BLEU/ROUGE**

---

##  Παραδοτέο 2 – Υπολογιστική Ανάλυση

- Word2Vec, GloVe, FastText, BERT
- Υπολογισμός cosine similarity μεταξύ αρχικού και τελικού
- Οπτικοποίηση ενσωματώσεων με PCA/t-SNE

---

##  Παραδοτέο 3 – Δομημένη Αναφορά

- Περιλαμβάνεται στο αρχείο `Παραδοτέο_3_Αναφορά.docx`
- Αναλύεται η μεθοδολογία, αποτελέσματα, συζήτηση και συμπεράσματα

---

##  Bonus – Masked Clause Input

- Συμπλήρωση άρθρων Αστικού Κώδικα με Masked Language Modeling
- Χρήση GreekBERT, RoBERTa και ανάλυση ακρίβειας
- Βλ. `Bonus_Masked_Clause_Report.docx`

---

##  Τεχνολογίες

- Python >= 3.10
- Poetry (για διαχείριση εξαρτήσεων)
- HuggingFace Transformers, spaCy, Gensim, scikit-learn, matplotlib
- Conda περιβάλλον

---

##  Εκτέλεση

1. Κλωνοποίηση:
```bash
git clone https://github.com/your-username/semantic-reconstruction-nlp.git
cd semantic-reconstruction-nlp
```

2. Δημιουργία περιβάλλοντος Conda:
```bash
conda create -n nlp-project python=3.10
conda activate nlp-project
poetry install
```

3. Εκτέλεση των scripts:
```bash
python scripts/reconstruction_pipeline.py
```

---

##  Σημειώσεις Ασφαλείας

- Το `.env` αρχείο περιέχει API κλειδιά (π.χ. HuggingFace) και πρέπει να **μην παρακολουθείται από το Git**.
- Συμπεριλαμβάνεται `.gitignore` για να προστατευθούν προσωπικά ή εμπιστευτικά δεδομένα.

---

##  Άδειες και Βιβλιογραφία

Για κάθε βιβλιοθήκη χρησιμοποιούνται οι αντίστοιχες open-source άδειες. Η βιβλιογραφία αναφέρεται στο Word report.
