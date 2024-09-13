git clone https://github.com/seu-usuario/flask-app.git
cd flask-app
python3 -m venv venv
source venv/bin/activate  # No Windows use `venv\Scripts\activate`
pip install Flask
from flask import Flask

app = Flask(__name__)

@app.route('/')
def home():
    return "Hello, Flask!"

if __name__ == '__main__':
    app.run(debug=True)
git add .
git commit -m "Initial commit with Flask app"
git push origin main
python app.py
