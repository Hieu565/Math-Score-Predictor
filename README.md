# Math-Score-Predictor
This project is an AI-powered learning assistant designed to help students analyze information, summarize content, and generate study support in real time. Built using Streamlit for the frontend interface, the app connects to a secure backend service that performs advanced model inference.

## 🔍 Purpose
This project is part of my university application portfolio, demonstrating skills in:
- Machine Learning
- Software Engineering
- Human-computer interaction
- Cloud Application Deployment

## 🚀 Project Goals
- Collect student data through a survey (hours studied, homework completion, focus level, past scores).
- Clean and process the dataset for machine learning.
- Build a predictive model (using regression) to estimate scores.
- Generate study improvement suggestions based on the model.

## ✨ Key Features
- ✅ Interactive AI Chat for question answering
- ✅ Automatic content summarization (text and media)
- ✅ Mind map style learning support
- ✅ Fast and intuitive user interface
- ✅ Accessible from any device via browser

## 📝 Survey Questions (Data Collection)
Question form: https://docs.google.com/forms/d/e/1FAIpQLSdhQQZbxIyvydRmxXZXAxtk96xiO3X16f8TzAdr_8Gyw6KPlA/viewform?usp=dialog

Questions:
- What was your average Math score (Coefficient I) in August?
- On average, how many hours per day do you spend self-studying Math at home?
- On average, what percentage of assigned Math homework do you complete?
- In each class session, what percentage of time do you spend focusing on the lesson?
  + (Focus = not using your phone, not sleeping, taking full notes)
- What methods do you prefer to use to learn maths?
- What methods do you use to solve difficult maths questions?
- Do you keep a study routine for self-studying maths?
- Do you often review before tests?
 
## 📊 Data Types

- Number of response: 152 students
- Data source is in this link: [[[https://docs.google.com/spreadsheets/d/1a-1Hwk_KpkGAfGQPWWlpINY8tcBKXkOlhXmfP1S6tZw/edit?usp=sharing](https://docs.google.com/spreadsheets/d/1i4An58zvSKWTDBqse78q5-pfQzc4uD9x-RS5I4sd6zk/edit?gid=0#gid=0)](https://docs.google.com/spreadsheets/d/1i4An58zvSKWTDBqse78q5-pfQzc4uD9x-RS5I4sd6zk/edit?gid=0#gid=0)](https://docs.google.com/spreadsheets/d/13f0_u9eZR8m7Ro36jfQCs35fGCWubqjwil3Jdfbkwao/edit?usp=sharing)
  
- 🔢 **Quantitative Data**
  + Math scores in August
  + Average self-study hours at hour
  + Estimate percentage range of homework completion
  + Estimate percentage range of attendance at class
- 📝 **Qualitative Data**
  + Prefered learning methods of student
  + Consistency of study habits (regular vs. cramming before tests)
  + Problem-solving approach when facing difficult math tasks

## 🧩 Architecture

This repository contains only the frontend Streamlit application.
User  →  Streamlit App (UI)  →  Secure Backend API  →  AI Model

🔒 The trained models and backend logic are stored in a private repository for security and intellectual property protection.

## 🛠️ Technologies Used
| Component | Technology                        |
| --------- | --------------------------------- |
| Frontend  | Streamlit                         |
| Backend   | FastAPI (private)                 |
| Model     | Custom fine-tuned model (private) |
| Language  | Python                            |
| Hosting   | Streamlit Cloud                   |

## 🚀 Live Demo
- 👉 Try the app here: https://math-score-prediction-ngkn3u3ymbtgktsjvb549t.streamlit.app/

## 📌 Limitations
- Data is self-reported, which may introduce bias.
- Small dataset may not generalize to all students.
- More features (sleep, tutoring, resources used) could improve accuracy.

## 📚 Future Improvements
- User authentication
- Learning analytics dashboard
- More adaptive response generation
- Voice input/output features

## 🤝 Contributing
- Fork the repo and submit pull requests.
- Share ideas for better features and models.

## 📜 License
MIT License. Free to use and modify.

## 📩 Contact
If you’d like to learn more about the backend implementation, trained models, or research behind the project, feel free to reach out:
- 📧 Email: phamminhhieu0817@gmail.com or hieu.m032108@gmail.com
- 🌍 Portfolio / LinkedIn: (https://www.linkedin.com/in/hi%E1%BA%BFu-ph%E1%BA%A1m-55a968385/)
