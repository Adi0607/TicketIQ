TicketIQ: AI-Powered Performance Evaluator
TicketIQ is an AI-driven system that automatically evaluates employee performance based on Jira ticket data.
It fetches ticket details, analyzes the work quality using Google Generative AI (Gemini), and generates detailed evaluation reports.

Features
🔗 Jira ticket integration

🗂️ MongoDB for ticket and user data storage

🤖 Work quality analysis via Google Gemini API

📄 Automated PDF report generation



Tech Stack
Backend: Java (Spring Boot), MongoDB

Analysis: Python, Google Generative AI


Project Structure

TicketIQ/
├── backend/         # Java Spring Boot backend
├── analysis/        # Python scripts for analysis and PDF generation
├── streamlit_app/   # Streamlit UI (optional)
└── README.md
Getting Started->

Backend
cd backend
# Configure application.properties
mvn clean install
mvn spring-boot:run

Analysis
cd analysis
pip install -r requirements.txt
python fetch_data.py
python analyze_tickets.py
python generate_pdf.py


How It Works
Java backend fetches Jira tickets and stores them in MongoDB.

Python scripts analyze the work using AI and generate evaluation reports
