# Auto-Comment Generator using AI

An AI-powered tool that generates meaningful comments for code snippets written in Python, C++, and Java.
It comes with:
1. A Flask backend API for programmatic access.
2. A Streamlit frontend UI for an interactive experience.

🚀 Features
1. Generate comments for Python, C++ and Java code.
2. Simple REST API endpoints.
3. Clean Streamlit interface with Lottie animations.
4. Modular code structure for easy extension.

📂 Project Structure
Auto_Comments-main
├── routes
│   ├── cpp_route.py
│   ├── java_route.py
│   ├── main_route.py
│   └── python_route.py
├── src
│   ├── cpp
│   ├── java
│   └── python
├── static
│   └── type_lottie.json
├── LICENSE
├── README.md
├── app.py          # Streamlit UI
├── requirements.txt
├── server.py       # Flask API server

⚙️ Installation
1. Clone the repository:
   git clone https://github.com/your-username/auto-comments.git
   cd auto-comments

2. Create and activate a virtual environment:
   python -m venv venv
   source venv/bin/activate   # Mac/Linux
   venv\Scripts\activate      # Windows

3. Install dependencies:
   pip install -r requirements.txt

▶️ Usage
Option 1 – Run Streamlit UI
  streamlit run app.py
  Open in browser: http://localhost:8501
  Paste your code.
  Select language (Python / C++ / Java).
  Click Generate Comments.

Option 2 – Run Flask API
  python server.py
  Server runs at: http://127.0.0.1:5000

Available endpoints:
  /python → Generate comments for Python code
  /cpp → Generate comments for C++ code
  /java → Generate comments for Java code

📌 Example (API)
  POST → /python
  {
    "code_snippet": "def add(a, b): return a + b"
  }

Response:
  # Function to add two numbers
  def add(a, b):
      return a + b

🎨 UI Preview
  Landing page shows an animation when no language is selected.
  Paste your code in the text area.
  Get instant AI-generated comments.

🛠️ Tech Stack
  Backend: Flask
  Frontend: Streamlit + Lottie animations
  Languages Supported: Python, C++, Java
