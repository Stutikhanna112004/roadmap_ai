# 🧭 AI Roadmap Generator

An AI-powered web application that generates personalized learning roadmaps based on a user's goals, current skill level, and time commitment. Built with **Flask** and powered by the **Groq API**.



## ✨ Features

- 🎯 **Personalized Roadmaps** — Generates a step-by-step learning path tailored to the user's goal
- 🤖 **AI-Powered** — Uses Groq's LLM API to dynamically generate structured, relevant content
- 🎨 **Simple Web UI** — Single-page interface (Flask + Jinja2 template) to enter a goal and view the generated roadmap
- ⚡ **Fast Inference** — Groq's LPU-based API returns responses quickly compared to typical LLM APIs



## 🛠️ Tech Stack

| Layer      | Technology              |
|------------|---------------------------|
| Backend    | Flask (Python)           |
| AI/LLM     | Groq API                 |
| Frontend   | HTML (Jinja2 templates)  |
| Config     | python-dotenv (.env)     |
| Deployment | Gunicorn-ready (Render / Railway) |



## 📂 Project Structure


roadmap_ai/
│
├── app.py                # Main Flask app — routes + Groq API logic
├── templates/
│   └── index.html        # Frontend page (form + roadmap display)
│
├── requirement.txt       # Python dependencies
├── .env                  # Environment variables (GROQ_API_KEY, etc.) — not committed
├── .gitignore
└── README.md




## ⚙️ Installation & Setup

### 1. Clone the repository
```bash
git clone https://github.com/<your-username>/roadmap_ai.git
cd roadmap_ai
```

### 2. Create a virtual environment
```bash
python -m venv venv
venv\Scripts\activate      # Windows
source venv/bin/activate   # macOS/Linux
```

### 3. Install dependencies
```bash
pip install -r requirement.txt
```

### 4. Set up environment variables
Create a `.env` file in the root directory:
```env
GROQ_API_KEY=your_groq_api_key_here
FLASK_ENV=development
SECRET_KEY=your_secret_key
```
Get a free Groq API key from [console.groq.com](https://console.groq.com).

### 5. Run the app
```bash
python app.py
```
Visit `http://127.0.0.1:5000` in your browser.



## 🚀 Usage

1. Open the app in your browser
2. Enter your learning goal (e.g., *"Become a Machine Learning Engineer"*)
3. Optionally specify current level and time available
4. Click **Generate Roadmap**
5. View your AI-generated, step-by-step roadmap on the same page



## 🔮 Future Improvements

- [ ] Save/export roadmap as PDF or Markdown
- [ ] Add user input validation & loading states in UI
- [ ] Support multiple LLM providers with fallback (Groq → Gemini/Ollama)
- [ ] Progress tracking with a checklist for each roadmap step
- [ ] Deploy live demo (Render/Railway) and link here



## 🤝 Contributing

Contributions and suggestions are welcome — feel free to open an issue or PR.



## 📄 License

This project is licensed under the MIT License.



## 👤 Author

**Stuti Khanna**
Final Year CSE(AI) Student | BBD University, Lucknow
