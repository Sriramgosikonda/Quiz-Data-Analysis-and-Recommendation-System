# **Personalized Student Recommendations**

## **Project Overview**

This project analyzes quiz performance data to provide personalized recommendations for students to improve their preparation. Using Python, we extract insights from both current and historical quiz data to highlight strengths, weaknesses, performance trends, and areas requiring improvement. The application is tailored for the **NEET Testline** app and offers actionable recommendations for students.

---

## **Key Features**
- **Data Analysis**: 
  - Extracts and processes current and historical quiz data.
  - Analyzes patterns in student performance by topics, difficulty levels, and accuracy.
- **Insight Generation**:
  - Highlights weak areas, performance gaps, and trends in accuracy.
  - Provides creative labels to identify strengths and weaknesses.
- **Personalized Recommendations**:
  - Suggests topics, question types, and difficulty levels to focus on for improvement.
- **Student Persona Creation**:
  - Defines personalized learning personas based on the analyzed data.

---

## **Technologies Used**
- **Language**: Python
- **Libraries**:
  - **Data Manipulation**: pandas, numpy
  - **Visualization**: matplotlib, seaborn
  - **Others**: json, datetime

---

## **Data Sources**
1. **Current Quiz Data**:
   - User's latest quiz submission details: `questions`, `topics`, `responses`, etc.
   - Data Source: Quiz API Endpoint.
   
2. **Historical Quiz Data**:
   - Data for the last 5 quizzes, including `scores` and `response map` (Key: Question ID, Value: Selected Option ID).
   - Data Source: Historical Quiz API Endpoint.

---

## **Setup Instructions**
1. **Clone the Repository**:
   ```bash
   git clone https://github.com/YourUsername/Personalized-Student-Recommendations.git
   cd Personalized-Student-Recommendations
python -m venv venv
source venv/bin/activate   # For Mac/Linux
venv\Scripts\activate      # For Windows
pip install -r requirements.txt
python main.py
Personalized-Student-Recommendations/
│
├── data/
│   ├── current_quiz_data.json  # Sample data for current quiz
│   └── historical_quiz_data.json  # Sample data for historical quizzes
│
├── src/
│   ├── data_preprocessing.py  # Handles data cleaning and transformation
│   ├── analysis.py  # Generates insights and trends
│   ├── recommendations.py  # Creates personalized recommendations
│   └── visualizations.py  # Plots charts and graphs
│
├── config.py  # Configuration file for API endpoints and settings
├── main.py  # Main script to run the analysis
├── requirements.txt  # Python dependencies
└── README.md  # Project description
