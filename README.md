# Language Translator

A hybrid rule‑based + machine‑learning translator between English and Italian.

[![CI Build Status](https://github.com/charliemunro/Language-translator/actions/workflows/ci.yml/badge.svg)](https://github.com/charliemunro/Language-translator/actions/workflows/ci.yml)  
[![PyPI Version](https://img.shields.io/pypi/v/language-translator)](https://pypi.org/project/language-translator/)  
[![License: MIT](https://img.shields.io/badge/license-MIT-blue)](LICENSE)  

---

## 📖 Overview

This package combines rule‑based NLTK preprocessing with a TensorFlow model to translate text between English and Italian. It offers:

- A **Python package** for programmatic translation  
- A **CLI** for quick one‑off translations  
- A **Flask web demo** for interactive use  

---

## 🚀 Installation

```bash
# 1. Clone this repository
git clone https://github.com/charliemunro/Language-translator.git
cd Language-translator

# 2. (Optional) Create a virtual environment
python3 -m venv venv
source venv/bin/activate

# 3. Install dependencies
pip install -r requirements.txt
# or install as a package:
pip install .
```

---

## 🎯 Quickstart

### CLI

```bash
# Translate a simple sentence
python cli.py --input "Hello, how are you?"
# → Ciao, come stai?
```

### Flask Demo

```bash
export FLASK_APP=app.py
flask run
# Then visit http://localhost:5000 in your browser
```

<p align="center">
  <img src="docs/demo-screenshot.png" alt="Flask demo screenshot" width="600"/>
</p>

---

## 🛠️ Package API

```python
from translator.model import Translator

# Initialize with your model/data paths
tr = Translator(model_path="data/eng_ita_model.h5")

# Translate text programmatically
print(tr.translate("Good morning"))  # → Buongiorno
```

---

## 🔧 Testing & CI

We use **pytest** for smoke tests and **GitHub Actions** to lint & run tests on every push.

```bash
# Run all tests locally
pytest
```

---

## 🤝 Contributing

Contributions welcome! Please check out [CONTRIBUTING.md](CONTRIBUTING.md) for guidelines on how to report issues or submit pull requests.

---

## 📄 License

This project is licensed under the **MIT License**. See the [LICENSE](LICENSE) file for details.

---

## 🔖 Topics

`python` · `nlp` · `flask` · `tensorflow` · `machine-learning`
