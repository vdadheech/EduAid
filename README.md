##🌉 EduAid: The Bridge Between Students and NGOs to Provide Them Aid
📊 Student Retention Prediction & Intervention Platform
🌟 Mission Statement
EduAid is a data-driven platform designed to act as a crucial bridge between vulnerable students and the Non-Governmental Organizations (NGOs) best equipped to provide targeted aid. By leveraging Machine Learning to predict which students are at the highest risk of dropping out, we enable NGOs to intervene proactively, ensuring every student has the support they need to succeed.

💡 The Problem & The Solution
The Problem: Student dropout is a global issue often stemming from socio-economic factors, lack of resources, and academic struggles. By the time a student's distress is noticed, it is often too late for effective intervention.

The Solution: EduAid uses predictive modeling on student data to identify potential dropouts early. This allows educators and partner NGOs to switch from reactive measures to proactive, targeted support—delivering the right aid (financial, tutoring, material) to the right student at the right time.

🚀 Key Features
Feature	Description	Technical Implementation
Dropout Prediction	A robust Machine Learning model that classifies students into risk categories (High, Medium, Low).	dropout_model.pkl (Serialized model) and model.py (Model training/loading).
NGO Matching	A system to securely share anonymized or aggregated student need profiles with verified NGO partners.	Integrated within app.py logic and database (to be implemented).
Intervention Dashboard	A web interface for educators to input student data, view prediction scores, and initiate an aid request ticket.	app.py (Flask framework) and files in the templates directory.
Data Security	Secure handling of student academic and demographic data for training and prediction.	Database setup and configuration in instance/ (requires user implementation).

Export to Sheets

🛠️ Local Setup and Installation
This project is built using Python, the Flask web framework, and popular data science libraries.

Prerequisites
Python 3.8+

pip (Python package installer)

Installation Steps
Clone the Repository:

Bash

git clone https://github.com/vdadheech/EduAid.git
cd EduAid
Create and Activate a Virtual Environment (Recommended):

Bash

python -m venv venv
source venv/bin/activate  # On Linux/macOS
# venv\Scripts\activate   # On Windows
Install Dependencies:

Create a requirements.txt file (if one doesn't exist) based on the project's use of Flask, Pandas, Scikit-learn, etc., and run:

Bash

pip install -r requirements.txt
(Note: The core dependencies appear to be Flask, pandas, and scikit-learn.)

Run the Application:

Start the Flask web server:

Bash

python app.py
Access the Platform:

Open your web browser and navigate to: http://127.0.0.1:5000/

📂 Project Structure
File/Folder	Purpose
app.py	The main Flask application file. Handles routing, web requests, and calls the prediction model.
model.py	Contains the code for training, evaluating, and saving the Student Retention Model.
data.py	Used for data loading, cleaning, and preprocessing (student_data.csv).
student_data.csv	Sample dataset used for training and testing the prediction model.
dropout_model.pkl	The trained and serialized Machine Learning model for instant prediction.
templates/	HTML files for the web interface (dashboard, input form, results).
static/	CSS, JavaScript, and image files for frontend styling.

Export to Sheets

🤝 Partnership & Collaboration
This is where the "bridge" is built.

NGOs interested in receiving targeted intervention requests based on our predictions should contact the project maintainers. Students or educators can also contribute by:

Improving the Model: Providing access to more diverse and verified data sets for better prediction accuracy.

Developing the Platform: Contributing to the web interface (templates, static files) or improving the app.py logic.

Testing: Thoroughly testing the application and reporting bugs/issues.

🔗 Connect
Project Repository: https://github.com/vdadheech/EduAid
