# CodFix

CodFix is an AI-powered application designed to assist developers with **code completion**, **debugging**, and **testcase generation** in **JAVA**.  
It consists of a **React frontend** for user interaction and a **Python backend** for model training and execution.

---

## 📁 Project Structure
CodFix/
│
├── public/
│ ├── index.html # Main HTML file
│ └── project_icon.png # Application icon
│
├── src/
│ ├── components/
│ │ ├── EditorPanel.js # Code editor UI
│ │ ├── EditorPanel.css
│ │ ├── Navbar.js # Navigation bar
│ │ ├── Navbar.css
│ │ ├── OutputPanel.js # Output display
│ │ ├── OutputPanel.css
│ │ ├── Tabs.js # Tabs for features
│ │ └── Tabs.css
│ │
│ ├── App.js # Root React component
│ ├── App.css
│ ├── index.js # React entry point
│ ├── project_icon.png
│ └── setupProxy.js # Proxy for backend API calls
│
├── App.py # Python backend entry point
│
├── code_completion_training.py # Code completion model training
├── debugging_training.py # Debugging model training
├── testcase_generation.py # Testcase generation logic
├── scrapping.py # Dataset preprocessing
│
├── requirements.txt # Python dependencies
├── package.json # React dependencies
├── package-lock.json
└── README.md

---

## 🛠 Prerequisites
Make sure the following are installed:
- **Python 3.8+**
- **Node.js (v16+)**
- **npm**
- **pip**

---

## ⚙️ Installation & Setup
### 1️⃣ Clone the Repository
```bash
git clone https://github.com/nreddyg07/CodFix.git
cd CodFix
```

### 2️⃣ Create Virtual Environment
**Linux / macOS**
```bash
python3 -m venv venv
source venv/bin/activate
```

```bash
**Windows**
python -m venv venv
venv\Scripts\activate
```

### 3️⃣ Install Python Dependencies
```bash
pip install -r requirements.txt
```

### 4️⃣ Install Node Dependencies
```bash
npm install
```

## 🚀 Running the Application
CodFix uses concurrently to run both the React frontend and Python backend at the same time.
### ▶️ Start Frontend + Backend Together
```bash
npm start
```

This single command will:
- Start the React frontend using react-scripts
- Start the Python backend by running App.py
- Automatically handle communication between frontend and backend

🌐 Access the Application
Once started, open your browser at:
```bash
http://localhost:3000
```
The backend runs internally and is proxied to the frontend.

## 🧠 Model Training

> **Important:**  
> All model training for CodFix was performed in **Google Colab** and is **not intended to be executed locally**.

The following scripts were used **only in Google Colab** for dataset preparation and model training:

- `scrapping.py` — Dataset scraping and preprocessing  
- `code_completion_training.py` — Code completion model training  
- `debugging_training.py` — Bug detection and debugging model training  
- `testcase_generation.py` — Automatic testcase generation  

These scripts require GPU acceleration and large compute resources, which is why they were executed in Google Colab.
