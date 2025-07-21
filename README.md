🔤 AutoCorrect Suggestion Web App
A simple web application built with Flask that provides word suggestions based on user input using Jaccard similarity and word probabilities from a text corpus.

📌 Features
Suggests words similar to the input keyword using Jaccard distance (q=2).

Ranks suggestions based on both similarity score and word probability.

Reads from a custom .txt file for building the vocabulary and frequency model.

Clean and minimal interface using Flask + HTML templates.

🚀 Demo
Type any misspelled word, and the app suggests corrections ranked by likelihood and similarity.

🛠️ Technologies Used
Python 🐍

Flask 🌐

Pandas 📊

TextDistance 🔤

Regular Expressions (re) 🧵

HTML + Jinja2 for frontend

📁 File Structure
php
Copy
Edit
.
├── app.py                      # Main Flask application
├── autocorrect book.txt       # Text corpus used to train the word model
├── templates/
│   └── index.html             # Frontend template
├── static/                    # (optional) for custom CSS/JS
├── README.md                  # This file
📚 How It Works
Corpus Loading: The app reads the file autocorrect book.txt, processes all words, and creates a frequency dictionary.

Probability Model: Calculates the probability of each word occurring.

Similarity Check: On receiving a keyword, it calculates Jaccard similarity with known words.

Suggestion Ranking: Suggestions are sorted based on similarity and frequency.

⚙️ How to Run Locally
Clone the repository:

bash
Copy
Edit
git clone https://github.com/your-username/autocorrect-flask-app.git
cd autocorrect-flask-app
Create a virtual environment and activate it:

bash
Copy
Edit
python -m venv venv
source venv/bin/activate  # On Windows use: venv\Scripts\activate
Install dependencies:

bash
Copy
Edit
pip install -r requirements.txt
requirements.txt

txt
Copy
Edit
flask
pandas
textdistance
Run the app:

bash
Copy
Edit
python app.py
Open your browser and go to:

cpp
Copy
Edit
http://127.0.0.1:5000
📝 Sample Input
Input: speling

Output Suggestions: spelling, spieling, splint, ...

✅ To Do
Add spelling correction using edit distance (like Levenshtein).

Support larger text corpora.

Add real-time suggestions with JavaScript (AJAX).

📄 License
This project is licensed under the MIT License.

🤝 Contributing
Pull requests are welcome. For major changes, please open an issue first to discuss what you would like to change.
