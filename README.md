# Language Translator

A bilingual translation pipeline between English and Italian, implemented entirely within a Jupyter Notebook.

---

## 📁 Project Structure

```
Language-translator/
├── eng_data.csv           # English training data
├── ita_data.csv           # Italian training data
├── sample_words.txt       # Sample English test sentences
├── sample_words_ita.txt   # Sample Italian test sentences
├── translator.ipynb       # Jupyter Notebook containing the full pipeline
└── README.md              # This file
```

---

## 🛠 Installation

1. **Clone the repository**  
   ```bash
   git clone https://github.com/charliemunro/Language-translator.git
   cd Language-translator
   ```

2. **Set up a virtual environment (optional but recommended)**  
   ```bash
   python3 -m venv venv
   source venv/bin/activate
   ```

3. **Install dependencies**  
   ```bash
   pip install pandas nltk tensorflow numpy scikit-learn matplotlib jupyter
   ```

---

## 🚀 Usage

1. **Launch the Jupyter Notebook**  
   ```bash
   jupyter notebook translator.ipynb
   ```
2. **Run through the cells** to:
   - Load and preprocess the English and Italian datasets.
   - Train the translation model using statistical or ML methods.
   - Evaluate performance on the sample test sentences.
   - Translate custom English sentences to Italian and vice versa.

3. **Modify or extend** the notebook by:
   - Adding new datasets in `eng_data.csv` / `ita_data.csv`.
   - Experimenting with different model architectures.
   - Visualizing results with matplotlib.

---

## 🗂 Data

- **eng_data.csv** & **ita_data.csv**: Parallel corpora for training.
- **sample_words.txt** & **sample_words_ita.txt**: Test pairs for quick evaluation.

---

## ⚙️ Next Steps

To make this project production-ready for employers:

- **Modularize** the code into Python packages (`translator/`).
- **Add a CLI** and **Flask web demo**.
- **Write unit tests** and configure **CI/CD** (GitHub Actions).
- **Include documentation** and project metadata (`setup.py`, `requirements.txt`, `LICENSE`).

---

## 📄 License

This project is licensed under the MIT License. See [LICENSE](LICENSE) for details.
