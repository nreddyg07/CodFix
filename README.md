# 🧠 CodFix – AI-Powered Code Intelligence Platform

CodFix is a full-stack AI-powered web application designed to assist developers with **intelligent code completion**, **bug detection and debugging**, and **automatic testcase generation**. By leveraging pre-trained machine learning models and an interactive web interface, CodFix streamlines common software development tasks and improves coding efficiency and reliability.

The system integrates a **React-based frontend** for seamless user interaction with a **Python backend** that serves pre-trained AI models for real-time inference, making advanced code intelligence accessible through a single unified platform.

---

## 📌 Project Overview

Modern software development involves repetitive tasks such as writing boilerplate code, debugging errors, and manually creating testcases. These tasks are time-consuming and error-prone.

CodFix addresses the following challenges:
- Manual effort in writing and completing code
- Time-consuming bug identification and debugging
- Lack of automated testcase generation
- Fragmented tooling for development assistance

By combining AI-driven models with a user-friendly interface, CodFix provides an end-to-end solution for improving developer productivity.

---

## ✨ Key Features

- **Code Completion** – Predicts and completes code snippets intelligently  
- **Bug Debugging Assistance** – Identifies potential bugs and suggests fixes  
- **Automatic Testcase Generation** – Generates relevant testcases for given code  
- **Integrated Web Interface** – Interactive editor and output panels  
- **Pre-trained AI Models** – Fast inference without local model training  
- **Single Command Execution** – Frontend and backend run together  

---

## 🏗️ Tech Stack

### Backend
- Python 3.8+
- FastAPI (API handling)
- Machine Learning models (pre-trained)
- NumPy, Pandas (data handling)

### Frontend
- React.js
- JavaScript (ES6+)
- HTML5 & CSS3

### Tools & Utilities
- concurrently (to run frontend & backend together)
- npm

---

## 📁 Project Structure

```

CodFix/
│
├── public/
│   ├── index.html                  # Main HTML file
│   └── project_icon.png            # Application icon
│
├── src/
│   ├── components/
│   │   ├── EditorPanel.js           # Code editor UI
│   │   ├── EditorPanel.css
│   │   ├── Navbar.js                # Navigation bar
│   │   ├── Navbar.css
│   │   ├── OutputPanel.js           # Output display
│   │   ├── OutputPanel.css
│   │   ├── Tabs.js                  # Feature tabs
│   │   └── Tabs.css
│   │
│   ├── App.js                       # Root React component
│   ├── App.css
│   ├── index.js                     # React entry point
│   ├── project_icon.png
│   └── setupProxy.js                # Proxy for backend API calls
│
├── App.py                           # Python backend entry point
│
├── code_completion_training.py      # Code completion training script
├── debugging_training.py            # Debugging model training script
├── testcase_generation.py           # Testcase generation logic
├── scrapping.py                     # Dataset preprocessing
│
├── requirements.txt                 # Python dependencies
├── package.json                     # Frontend & concurrent scripts
├── package-lock.json
└── README.md

````

---

## ⚙️ Prerequisites

### Software
- Python 3.8 or higher
- Node.js 16 or higher
- npm
- Git

### Hardware
- Minimum: 8 GB RAM
- Recommended: 16 GB RAM or higher

---

## 🚀 Installation & Setup

### Clone the Repository

```bash
git clone https://github.com/nreddyg07/CodFix.git
cd CodFix
````

---

### Backend Setup (Python)

Create and activate a virtual environment:

**Windows**

```bash
python -m venv venv
venv\Scripts\activate
```

**Linux / macOS**

```bash
python3 -m venv venv
source venv/bin/activate
```

Install backend dependencies:

```bash
pip install -r requirements.txt
```

---

### Frontend Setup (React)

Install frontend dependencies:

```bash
npm install
```

---

## ▶️ Running the Application

CodFix uses **concurrently** to run both the frontend and backend together.

### Start the Application

```bash
npm start
```

This single command will:

* Start the React frontend
* Start the Python backend (`App.py`)
* Enable real-time communication between frontend and backend

---

### 🌐 Access the Application

Open your browser and navigate to:

```
http://localhost:3000
```

---

## 🧠 Model Training

> **Important:**
> All model training for CodFix was performed in **Google Colab** and is **not intended to be executed locally**.

The following scripts were used **only in Google Colab** for dataset preparation and training:

* `scrapping.py` — Dataset scraping and preprocessing
* `code_completion_training.py` — Code completion model training
* `debugging_training.py` — Bug detection and debugging model training
* `testcase_generation.py` — Automatic testcase generation

These scripts require GPU acceleration and large compute resources.

---

### 🚫 Do Not Run Training Scripts Locally

```bash
python scrapping.py
python code_completion_training.py
python debugging_training.py
python testcase_generation.py
```

The local application uses **pre-trained models only**.

---

---

## 📊 Dataset

The dataset used for training the CodFix models was collected and prepared using custom scraping and preprocessing scripts.

**Dataset Source:**  
🔗 [<DATASET_LINK>](https://drive.google.com/drive/folders/1c_y5aVEIcUV7rsGFOpFTKVVVxY_XwhcW?usp=drive_link)

### Dataset Description

The dataset consists of code snippets collected from various programming resources and repositories. It includes examples of:

- Correct code implementations
- Code with bugs and debugging examples
- Code snippets for completion tasks
- Programs used for testcase generation

### Dataset Preparation

The dataset was prepared using:

- `scrapping.py` — Collects and preprocesses code samples
- Cleaning and formatting of source code
- Structuring code snippets for training tasks such as:
  - Code completion
  - Debugging
  - Testcase generation

### Dataset Usage

The dataset was used during **model training in Google Colab** to train the following components:

- Code Completion Model
- Debugging Assistance Model
- Testcase Generation Model

Due to computational requirements, training was performed on **Google Colab GPU environments**.

---

## 🧪 Final Execution Flow

```bash
# One-time setup
pip install -r requirements.txt
npm install

# Run frontend + backend together
npm start
```

---

## 🌍 Applications

* Software development assistance
* Academic and student projects
* Automated testing workflows
* Developer productivity tools
* AI-assisted programming education

---

## 👨‍💻 Contributors

**Team Members**
- Gagana N  
- Harsh M Jain  
- Anish B  
- Dhanush R Gowda  

**Guided by**  
Dr. Hemavathi P  
Professor, CSE
Bangalore Institute of Technology

---

## 📜 License

This project is licensed under the **MIT License**.

---

## 📞 Support

For questions, issues, or feature requests, please open an issue on the GitHub repository.

---
