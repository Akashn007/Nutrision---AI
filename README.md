# Nutrision-AI 
Snap your food, get insights

This is a Flask-based web application that allows users to upload a food image and receive detailed nutritional analysis, personalized diet plans, and recommendations using Google's Gemini API.

---

## 🚀 Features

- User Registration & Login
- Upload food image
- Analyze image using Gemini API (multimodal AI)
- Get:
  - Food name
  - Nutritional breakdown
  - Suitability based on age, BMI, gender
  - Personalized diet plan & recommendation
- Store user health data & analysis in SQLite
- User dashboard with BMI calculation

---

## 🛠️ Tech Stack

- Python + Flask
- SQLite (SQLAlchemy ORM)
- HTML + Bootstrap (Jinja templates)
- Gemini 2.0 Flash API (for food recognition)

---

## 📁 Project Structure

nutrition_project/
│
├── app.py # Main Flask app
├── instance/
│ └── users.db # SQLite database
├── uploads/ # Uploaded food images
├── templates/ # HTML files
│ ├── login.html
│ ├── register.html
│ ├── dashboard.html
│ └── result.html
└── README.md


## 🧪 Setup Instructions

### 1. Clone this repo

git clone https://github.com/yourusername/nutrition-project.git
cd nutrition-project
### 2. Create virtual environment (optional but recommended)


python -m venv venv
venv\Scripts\activate        # On Windows
source venv/bin/activate     # On macOS/Linux
### 3. Install dependencies
pip install flask flask_sqlalchemy werkzeug requests

### 4. Run the app
python app.py
Visit http://127.0.0.1:5000 in your browser.

🔐 Gemini API Setup
Replace the placeholder in app.py with your own Gemini API Key:

python
Copy code
API_KEY = "YOUR_ACTUAL_GEMINI_API_KEY"
You can get a key from: https://makersuite.google.com/app

✅ To-Do
Add user food history view

Graphs for BMI trend

Admin dashboard

Dockerize the app



📄 License
MIT License © 2025 Akash N
