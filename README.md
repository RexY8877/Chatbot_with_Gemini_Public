# My Corporate School – Customer Support Chatbot

This project is a **customer support chatbot** for [My Corporate School](https://mycorporateschool.com).  
It answers FAQs using a custom knowledge base and, when needed, falls back to **Google Gemini** via the `google-generativeai` SDK. The backend is powered by **Flask**, and the frontend is a floating chat widget you can embed in any website. 

---

## ✨ Features

- FAQ-style responses using a local **Python knowledge base**. :contentReference[oaicite:1]{index=1}  
- Smart fallback to **Gemini 1.5 Flash** when the question is not in the FAQ. :contentReference[oaicite:2]{index=2}  
- REST API (`/chat`) to receive user messages and return bot replies. :contentReference[oaicite:3]{index=3}  
- **CORS-enabled** Flask backend (so it can talk to any frontend / domain). :contentReference[oaicite:4]{index=4}  
- Modern floating **chat widget UI** built in pure HTML + Tailwind CSS + JavaScript. :contentReference[oaicite:5]{index=5}  
- Ready for deployment on **Render.com** via `Render.yaml`.  
- Secrets handled with `.env` and ignored from git via `.gitignore`.   

---

## 🧱 Tech Stack

- **Backend:** Python, Flask, Flask-CORS   
- **AI:** Google Gemini (via `google-generativeai`)   
- **Frontend:** HTML, Tailwind CSS, Vanilla JavaScript :contentReference[oaicite:9]{index=9}  
- **Server:** gunicorn (for production) :contentReference[oaicite:10]{index=10}  
- **Config / Infra:** `.env`, `Render.yaml`, `.gitignore`   

---

## 📂 Project Structure

```text
.
├── Backend.py            # Flask backend + Gemini integration
├── Front_End.html        # Chat widget UI
├── YOUR_Knowledge_BASE.py# FAQ-style knowledge base
├── Requirements.txt      # Python dependencies
├── .env                  # Environment variables (NOT committed) 
├── .gitignore            # Git ignore rules
├── Render.yaml           # Render.com deployment config
└── README.md             # (You are here)
