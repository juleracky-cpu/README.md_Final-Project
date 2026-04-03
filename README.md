## Final Project: Flask Healthcare Application
# Income & Spending Survey Tool - Healthcare Product Launch

## Project Overview
This project is a complete data collection and analysis system developed for a healthcare company in Washington, DC. It collects participants' income and spending data (with special focus on healthcare expenses) through a web-based survey, stores the data in MongoDB, processes it using a custom Python class, exports it to CSV, and generates visualizations for client presentation.

These insights provide actionable intelligence to support targeted marketing and product positioning for the upcoming healthcare offering.

## Features Implemented
- Web Interface: Flask web application with user-friendly survey form
- Data Collection: Age, Gender, Total Income, and checkbox plus amount fields for 5 expense categories (Utilities, Entertainment, School Fees, Shopping, Healthcare)
- Data Storage: MongoDB for persistent storage
- Data Processing: Custom `User` Python class
- CSV Export: Automatic appending of survey responses to `data/users.csv`
- Data Analysis: Jupyter Notebook with required visualizations
- Export: High-resolution charts ready for PowerPoint
- Code Quality: Clean structure, proper error handling, and best practices

## Project Structure
income_spending_survey/
├── app.py                    # Flask web application
├── models                    
│   └── user.py               # User class for data processing
├── templates/
│   └── index.html            # Survey form
├── data/
│   └── users.csv             # Collected data (generated)
├── jupyter/
│   └── Analysis.ipynb        # Data analysis and visualizations
├── charts/                   # Exported charts for PowerPoint
│   ├── age_vs_income.png
│   ├── gender_spending.png
│   └── total_expenses_by_gender.png
├── requirements.txt
└── README.md                 # This file
└── export_data.py            # MongoDB → CSV

## Instructions
1. Install MongoDB
2. Install dependencies:
   ```bash
   pip install -r requirements.txt
3. Run the Flask app:
   Bash
   python app.py
4. Open browser and go to: http://127.0.0.1:5000/
5. Fill the survey multiple times to generate data
6. Open jupyter/analysis.ipynb to view analysis and generate charts

# Requirements.txt
Flask
pymongo
pandas
matplotlib
seaborn

# Visualizations for Client Presentation
Three high-resolution charts have been exported to the charts/ folder:
- age_vs_income.png → Average Total Income by Age
- gender_spending.png → Average Spending by Gender and Expense Category
- total_expenses_by_gender.png → Distribution of Total Expenses by Gender
These charts are ready to be inserted directly into the PowerPoint presentation.

# Deployment on AWS
Recommended: Use AWS EC2 (Ubuntu) + MongoDB Atlas
Connect Flask app to MongoDB Atlas connection string
Use Gunicorn + Nginx for production

# Technologies Used
- Python + Flask (Backend & Web)
- MongoDB (Database)
- Pandas, Matplotlib, Seaborn (Analysis & Visualization)
- Jupyter Notebook

# Notes
All assignment requirements have been fully addressed:
- Flask webpage for data collection
- MongoDB storage
- Python User class
- CSV export with loop through data
- Jupyter notebook visualizations
- Charts exported for PowerPoint
- Clean code with comments and best practices


Author:Jule Ahebwa
Date: 06th April 2026
Company: Data Analysis Company, Washington DC
