# 🔤 AutoCorrect Suggestion System

A simple web application built with Flask that provides word suggestions based on user input using Jaccard similarity and word probabilities from a text corpus.

---

## 📌 Features

Suggests words similar to the input keyword using Jaccard distance (q=2).

Ranks suggestions based on both similarity score and word probability.

Reads from a custom .txt file for building the vocabulary and frequency model.

Clean and minimal interface using Flask + HTML templates.

---

## 🛠️ Technologies Used

Python 🐍

Flask 🌐

Pandas 📊

TextDistance 🔤

Regular Expressions (re) 🧵

HTML + Jinja2 for frontend

---

## 📁 File Structure
.
├── app.py                      # Main Flask application

├── autocorrect book.txt       # Text corpus used to train the word model

├── templates/
│   └── index.html             # Frontend template

├── static/                    # (optional) for custom CSS/JS

├── README.md                  # This file


---

## 📚 How It Works

Corpus Loading: The app reads the file autocorrect book.txt, processes all words, and creates a frequency dictionary.

Probability Model: Calculates the probability of each word occurring.

Similarity Check: On receiving a keyword, it calculates Jaccard similarity with known words.

Suggestion Ranking: Suggestions are sorted based on similarity and frequency.

---

## ⚙️ How to Run Locally

Clone the repository:
git clone https://github.com/your-username/autocorrect-flask-app.git

cd autocorrect-flask-app

## Install dependencies:
pip install -r requirements.txt

## requirements.txt
flask
pandas
textdistance


## Run the app:
python app.py

## Open your browser and go to:
http://127.0.0.1:5000


## 📝 Sample Input
Input: speling

Output Suggestions: spelling, spieling, splint, ...


## 📄 License
This project is licensed under the MIT License.

## 🤝 Contributing
Pull requests are welcome. For major changes, please open an issue first to discuss what you would like to change.
