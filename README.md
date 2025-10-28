# Math-Score-Predictor
This project is an AI-powered learning assistant designed to help students analyze information, and generate study support in real time. Built using Streamlit for the frontend interface, the app connects to a secure backend service that performs advanced model inference.

## ✅ Why This Project Matters
This project demonstrates my ability to build a complete machine learning system — from data collection and feature engineering to model evaluation, deployment, and user experience design.

## 🔍 Purpose
This project is part of my university application portfolio, designed to:
- Demonstrate skills in **Machine Learning**, **Software Engineering**, and **Human-Computer Interaction**.
- Explore and satisfy **curiosity** about the relationship between study habits and math performance.
- Show practical understanding of **Cloud Application Deployment** and data-driven insight generation.

## 🚀 Project Goals
- Collect student data through a survey (hours studied, homework completion, focus level, past scores).
- Clean and process the dataset for machine learning.
- Build a predictive model (using regression) to estimate scores.
- Generate study improvement suggestions based on the model.

## ✨ Key Features
- 🎯 Score Prediction System (main ML component)
- 🧠 Learning Assistant Tool (interactive AI support)
- 📄 Automatic content summarization (text & media)
- ⚡ Fast and intuitive UI, accessible on any device

## 📝 Survey Questions (Data Collection)

Questions:
- What was your average Math score (Coefficient I) in August?
- On average, how many hours per day do you spend self-studying Math at home?
- On average, what percentage of assigned Math homework do you complete?
- In each class session, what percentage of time do you spend focusing on the lesson?
  + (Focus = not using your phone, not sleeping, taking full notes)
- What methods do you prefer to use to learn maths?
- What methods do you use to solve difficult maths questions?
- Do you keep a daily, weekly study routine or just review before test?
 
## 📊 Data Types

| Feature                       | Type                                | Description |
|------------------------------|-------------------------------------|-------------|
| MathScore                    | Numeric (0–10 scale)        | Final math score used for prediction |
| StudyHours                   | Numeric (hours/day)                 | Daily reported independent study time |
| HomeworkCompletion          | Categorical (0–100%)                | Predicts consistency and responsibility in learning |
| AttentionLevel     | Categorical (0–100%)                | Indicates attention and engagement during lessons |
| StudyRoutines      | Categorical (weekly, daily, before test) | Measures discipline and long-term learning habits |
| LearningMethods   | Multi-select Categorical            | Shows how students approach new content (e.g., videos, group work, notes) |
| HandleDifficultMethod  | Multi-select Categorical            | Strategies used when facing challenging material (e.g., ask teacher, online search, peer help) |

✅ Data & Ethics Disclosure
- 152 student responses were collected voluntarily
- Personal identifiers were not collected
- All data was fully anonymized before use
- Used only for educational and research purposes

- Data source is in this link: [Google Sheets](https://docs.google.com/spreadsheets/d/13f0_u9eZR8m7Ro36jfQCs35fGCWubqjwil3Jdfbkwao/edit?usp=sharing)

## 🧩 Architecture

This repository contains only the frontend Streamlit application.

User  →  Streamlit App (UI)  →  Secure Backend API  →  AI Model

🔒 The trained models and backend logic are stored in a private repository for security and intellectual property protection.

## 📈 Model Evaluation
Evaluate how accurately the regression model can predict a student’s Math score based on behavior and study habit features.

✅ Train–Test Split
+ Training set: 80%
+ Testing set: 20%
+ Cross-validation: 5-fold CV
This ensures the model generalizes well to unseen data.

📊 Detailed results are available here:  
👉 [Model Evaluation Report](https://github.com/Hieu565/Math-Score-Predictor/blob/main/Model_Results/Model%20Performance%20Report%20README.md)

📊 Evaluation Metrics

We use multiple metrics for a reliable assessment:
| Metric                             | Purpose                                  | Result         |
| ---------------------------------- | ---------------------------------------- | -------------- |
| **R² Score**                       | Measures variance explained by the model |      0.26      |
| **RMSE** (Root Mean Squared Error) | Penalizes larger errors                  |      1.28      |
| **Tolerance** (±1 point accuracy)  | Practical correctness within acceptable score deviation | 51.61% |

- Most prediction errors fall within ±1 points of the real score.
- R² and RMSE indicate that the model still struggles with generalization, likely due to the limited dataset and self-reported variability.
- The model achieves 51% accuracy within ±1 point on a 0–10 scale, which means more than half of the predictions are close to the actual scores.

Given the dataset’s size and self-reported nature, this serves as a reasonable baseline for educational prediction tasks. This means predictions are directionally reliable but not a replacement for formal assessment.

🔍 Feature Importance

The model found these features to be the most influential on predicted results:
- Attention Level during lessons
- Daily self-study hours
- Homework completion rate

This analysis supports educational insights — focusing and consistent practice strongly correlate with improved performance.

📉 Error Distribution

- The system is designed as a learning improvement tool, not a grading authority.
- Future improvements aim to raise this tolerance above 65% by expanding the dataset and including additional study-related variables.

## 🛠️ Technologies Used
| Component | Technology                        |
| --------- | --------------------------------- |
| Frontend  | Streamlit                         |
| Backend   | FastAPI (private)                 |
| Model     | Custom fine-tuned model (private) |
| Language  | Python                            |
| Hosting   | Streamlit Cloud                   |

## 🚀 Live Demo

- App UI interface:
<img width="1030" height="856" alt="image" src="https://github.com/user-attachments/assets/82a13107-c85f-456f-bba8-dfb9e342ef18" />
<img width="970" height="815" alt="image" src="https://github.com/user-attachments/assets/35cbb1bf-163c-41d5-9cff-4bef898b873e" />

- 👉 Try the app here: [Math Score Predictor App](https://math-score-prediction-ngkn3u3ymbtgktsjvb549t.streamlit.app/)
- 👉 Download the video demo here: [Math Score Predictor App](https://github.com/Hieu565/Math-Score-Predictor/blob/main/Math%20Score%20Predictor%20App%20Demo.mp4)

## 📌 Limitations
- Data is self-reported, which may introduce bias.
- Small dataset may not generalize to all students.
- More features (sleep, tutoring, resources used) could improve accuracy.

## 📚 Future Improvements
- Improve tolerance to above 65%
- Adding other features such as sleep hours, teaching quality to improve the model
- Add chatbot to improve user experience
- User authentication
- Learning analytics dashboard
- More adaptive response generation

## 🤝 Contributing
- Fork the repo and submit pull requests.
- Share ideas for better features and models.

## 📜 License
MIT License. Free to use and modify.

## 📩 Contact
If you’d like to learn more about the backend implementation, trained models, or research behind the project, feel free to reach out:
- 📧 Email: phamminhhieu0817@gmail.com or hieu.m032108@gmail.com
- 🌍 Portfolio / LinkedIn: [Hiếu Phạm](https://www.linkedin.com/in/hi%E1%BA%BFu-ph%E1%BA%A1m-55a968385/)
