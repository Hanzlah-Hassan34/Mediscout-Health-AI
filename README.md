# 🏥 MediScout Pakistan – AI for Early Diagnosis in Underserved Communities

**MediScout** is an AI-powered diagnostic tool designed to assist community health workers (CHWs) in underserved regions of Pakistan. It offers early risk triage and preliminary diagnosis of common illnesses through a lightweight web interface and predictive models.

---

## ✅ Features

- 📊 **Synthetic Data Simulation** (based on epidemiological stats from Pakistan)
- 🤖 **AI-Powered Risk Scoring**
- 📷 **Image Classification for Symptom Detection**
- 📝 **Free-Text Symptom Triage using NLP**
- 🚨 **High-Risk Case Flagging**
- 🌍 **Interactive Visualizations (AI vs Non-AI Outcomes, Disease Maps)**
- 📈 **Model Evaluation Metrics (ROC, Confusion Matrix, Accuracy, etc.)**
- 💡 **Smart Recommendations and Risk Interpretations**

---

## 🛠️ Tech Stack Used

- Python 3.10+
- Flask
- Scikit-learn
- Pandas, NumPy
- Streamlit (for dashboard)
- Matplotlib & Seaborn (for visualizations)
- PIL / OpenCV (for image processing)
- HTML, CSS (for web frontend)

---

## 🖼️ Screenshots

📌 

- `/screenshots/ui_home.png` – Patient input form
- `/screenshots/result_view.png` – Result display
  
  ![IMG-20250517-WA0012](https://github.com/user-attachments/assets/4b80bb54-3a04-4027-b999-9b4caff8e027)
  ![IMG-20250517-WA0013](https://github.com/user-attachments/assets/3b02ed65-ea64-497b-ba09-6360d913d288)
  ![IMG-20250517-WA0014](https://github.com/user-attachments/assets/aeb7a19b-91e4-48a4-80f9-5b7e321ddc32)

- `/screenshots/confusion_matrix.png` – Model performance
  ![Accuracy](https://github.com/user-attachments/assets/0a7bb326-3f09-47d6-a594-f97c4c76fb86)

- `/screenshots/ai_vs_nonai.png` – AI vs non-AI detection impact
  ![IMG-20250517-WA0007](https://github.com/user-attachments/assets/1441f742-6692-4bda-b139-69408164bab2)

- `/screenshots/roc_curve.png` – ROC visualization
  ![ROC](https://github.com/user-attachments/assets/dc64e7c9-fae2-47e5-a09e-a8611e09ab9c)

- `/screenshots/actual_vs_predicted.png` – Comparison graph
  ![IMG-20250517-WA0009](https://github.com/user-attachments/assets/4c4e1a75-5618-480d-81b4-233612fd5d90)

## 📁 Folder Structure

MediScout/
│
├── lastapp.py                        # Main Flask application

├── lastbalanced_model.pkl           # Trained RandomForest model

├── lastsimple_model_web.py          # Feature extraction logic

├── lastbalanced_model_trainer.py    # Model training script

├── evaluate_climate.py              # Climate impact evaluation

├── templates/

│   ├── index.html                   # Input UI

│   └── result.html                  # Output UI

├── static/

│   └── uploads/                     # Uploaded patient images

├── data/

│   ├── simulated_health_data.csv    # Synthetic patient records for training

│   ├── climate_dataset.csv          # External climate data (temperature, rainfall, etc.)

│   └── symptom_keywords.csv         # Keyword reference for symptom triage

├── evaluation_results/              # Model graphs & evaluations

├── medi_scout_output.csv            # Logs and predictions of inference cases

└── requirements.txt                 # Python dependencies


🧠 Problem Statement / Motivation
Access to early medical diagnostics remains a critical challenge in Pakistan’s rural and peri-urban regions. Seasonal surges in diseases like dengue, tuberculosis, ARIs, and maternal 

complications go undetected due to lack of tools. MediScout empowers CHWs with AI-assisted triage and diagnosis to reduce delays and enhance intervention — directly supporting SDG 3: 

Good Health and Well-being.

▶️ How to Run the Project

# Step 1: Clone the repo

git clone https://github.com/yourusername/mediscout.git

cd mediscout/

# Step 2: Install dependenciesM

pip install -r requirements.txt

# Step 3: Run the app
python lastapp.py

Navigate to http://127.0.0.1:5000/ in your browser.

👨‍💻 Team & Contributions

Salman Ahmad (BS SE) – UI/UX development, deployment configuration, and system design

Hanzlah Hassan (BS AI) – Model training, evaluation, and synthetic data generation

Awais Ali (BS AI) – Full-stack AI pipeline integration, frontend-backend interaction


🎓 Course / Context
🚀 Developed for a Hackathon organized by Capital University of Science & Technology (CUST)

📅 Spring 2025 | AI for Health Domain


📌 Extra Notes

🧪 Includes synthetic patient data modeled on real epidemiological assumptions (e.g., dengue spikes in monsoon)

📉 Evaluation visualizations include confusion matrix, ROC, AI vs Non-AI effectiveness, etc.

🧱 Full architectural breakdown includes:

Modular Flask app

Separate scripts for training & evaluation

Scalable, REST-ready endpoints

📊 System logs and stores every prediction for audit and analysis

🌐 Future-ready: roadmap includes SMS alerts, mobile app integration, and CHW workflow compatibility

“AI won’t replace doctors, but tools like MediScout will amplify their reach in communities that need it most.”
