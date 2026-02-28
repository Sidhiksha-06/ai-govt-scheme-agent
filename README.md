AI Government Scheme Awareness and Fraud Detection Agent;

Introduction:

  The AI Government Scheme Awareness and Fraud Detection Agent is a web-based application developed to assist citizens in identifying relevant government schemes based on their personal and socio-economic details. The system is designed to reduce the information gap between citizens and welfare programs by recommending schemes using a weighted eligibility scoring mechanism. 
Additionally, the application includes a fraud detection module that analyzes suspicious scheme-related messages and alerts users about potential scams.This project demonstrates the implementation of rule-based AI decision logic, eligibility ranking, fraud pattern detection, and administrative analytics within a public welfare domain.

Objectives:

  The primary objectives of this project are:
    1.To recommend government schemes based on user eligibility criteria.
    2.To rank schemes using a scoring-based evaluation model.
    3.To calculate estimated financial benefits available to the user.
    4.To detect fraudulent or suspicious scheme-related messages.
    5.To provide an administrative dashboard for monitoring system usage.

System Overview:

  The application consists of three major components:
    1.User Scheme Recommendation Module
    2.Fraud Detection Module
    3.Admin Analytics Dashboard
  The system uses a rule-based weighted scoring approach to evaluate eligibility conditions such as age, income, category, community, and state. Instead of strict filtering, schemes are ranked according to how closely they match the user’s profile.
Fraud detection is implemented using keyword and pattern-based logic to identify suspicious content, including urgency phrases, payment requests, and suspicious links.

Technologies Used:

Backend:
  Python
  Flask Framework
Frontend:
  HTML
  CSS
  JavaScript
  Data Storage:
  JSON-based data files
Visualization:
  Chart.js for analytics dashboard
Architecture:
  Rule-based AI scoring system

Project Structure:

│── app.py
│── schemes.json
│── fraud_schemes.json
│
├── templates/
│   ├── index.html
│   ├── admin.html
│
└── static/
    ├── style.css
    ├── script.js

Installation and Setup Procedure:

Step 1: Clone the Repository
  Open terminal and execute: git clone https://github.com/your-username/ai-government-scheme-agent.git
Step 2: Navigate to the Project Directory
  cd ai-government-scheme-agent
Step 3: Install Required Dependencies
  Ensure Python is installed, then run: pip install -r requirements.txt
Step 4: Run the Application : python app.py
Step 5: Access the Application
  Open your browser and go to:http://127.0.0.1:5000
  To access the admin dashboard:http://127.0.0.1:5000/admin

Working Procedure:

  1.The user enters personal details including age, annual income, category, community, and state.
  2.The system evaluates each scheme using predefined eligibility conditions.
  3.A weighted score is calculated for each scheme based on:
      Age eligibility
      Income condition
      Category relevance
      Community match
      State applicability
  4.Schemes are ranked according to their eligibility score.
  5.The system displays recommended schemes along with descriptions, required documents, and estimated benefit amounts.
  6.In the fraud detection module, users can paste suspicious messages. The system analyzes the content using predefined keywords and pattern checks, assigns a fraud risk score, and indicates whether the message appears fraudulent.
  7.The admin dashboard collects user interaction data and provides analytics including total users and the most common applicant category.

Fraud Detection Logic:

  The fraud detection module evaluates messages based on:
    *Suspicious keywords such as payment requests and urgency indicators.
    *References to processing fees or registration fees.
    *Suspicious URL patterns such as shortened links.
    *Combined keyword occurrences to generate a fraud risk score.
  If the fraud score crosses a predefined threshold, the system flags the message as potentially fraudulent.

Key Functional Features:

  Intelligent scheme recommendation using weighted scoring.
  Community and state-based eligibility refinement.
  Estimated benefit calculation.
  Fraud detection with risk scoring.
  Admin dashboard with usage analytics.
  Government-themed user interface.

Future Enhancements:

  Potential improvements for future development include:
    1.Integration with a relational database system.
    2.Machine learning-based fraud detection.
    3.User authentication and role management.
    4.Deployment on cloud platforms.
    5.Multi-language support.
    6.Advanced analytics and reporting features.

Conclusion:

  The AI Government Scheme Awareness and Fraud Detection Agent demonstrates how rule-based artificial intelligence logic can be applied to solve real-world public welfare challenges. By combining eligibility ranking, fraud detection, and administrative analytics within a simple web interface, the system improves accessibility, awareness, and digital safety for citizens. The project highlights practical implementation of AI-driven decision-making in a socially impactful domain.
