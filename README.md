# AI--Based---Recruitment---System
Project Description 📝
This project is an AI Recruitment System designed to accelerate the hiring process for HR and technical recruiters. The application allows recruiters to:

📄 Upload candidate resumes, job descriptions, job roles, and additional evaluation instructions.
🤖 Evaluate resumes using AI.
✉️ Automatically send email notifications to candidates with feedback, indicating whether they are selected or rejected.
📅 Schedule Zoom meetings for the next day as an initial round of interviews.
This system significantly streamlines the recruitment process by selecting the most suitable candidates and providing immediate feedback to candidates on areas for improvement.

Prerequisites ⚙️
To configure this application, the following credentials and accounts are required:

API Keys for LLM Models 🔑:
Obtain API keys from the official websites of Mistral, Claude, or OpenAI.
Gmail Account for Email Notifications 📧:
Create or use an existing Gmail account for the recruiter.
Enable 2-Step Verification and generate an App Password.
The app password is a 16-digit code generated through Google App Password.
Format: afec wejf awoj fwrv (use without spaces in the Streamlit app).
Zoom API Credentials 🎥:
Create or use an existing Zoom account.
Navigate to the Zoom App Marketplace and create a new app with Server-to-Server OAuth.
Obtain the following credentials:
Client ID
Client Secret
Account ID
Add the following scopes to the app for Zoom meeting scheduling:
meeting:write:invite_links:admin
meeting:write:meeting:admin
meeting:write:meeting:master
meeting:write:invite_links:master
meeting:write:open_app:admin
user:read:email:admin
user:read:list_users:admin
billing:read:user_entitlement:admin
dashboard:read:list_meeting_participants:admin (optional)
Installation 🛠️
Run Locally 💻
Clone this repository:

git clone https://github.com/manthan89-py/AI-Based-Recruitment-System.git
Ensure Python (version >= 3.10) is installed.

Install the UV package manager:

pip install uv
Navigate to the cloned repository:

cd AI-Based-Recruitment-System
Create a new virtual environment:

uv venv --python 3.10
Activate the environment:

On Linux/MacOS:
source .venv/bin/activate
On Windows:
.venv\Scripts\activate
Install dependencies:

uv install
Run the application:

streamlit run app.py
Run with Docker 🐳
Build Locally 🏗️
Build the Docker image:

docker build -t localmachine/ai_recruitment_team:main-latest .
Run the Docker container:

docker run -p 7860:7860 localmachine/ai_recruitment_team:main-latest
Use Prebuilt Image 📦
Pull the prebuilt image from DockerHub:

docker pull manthan07/ai_recruitment_team:main-latest
Run the Docker container:

docker run -p 7860:7860 manthan07/ai_recruitment_team:main-latest
Technologies Used 🛠️
PhiData: Agents (Resume Analyzer Agent, Email Agent, Scheduler Agent) and Tools (ZoomTool)
Python 🐍
Pydantic 📋
PyPDF2 📄
Streamlit 🌐
Features ✨
Automated Resume Analysis: 📄 Evaluate candidate resumes based on the provided job description.
Email Notifications: ✉️ Notify candidates of their selection status with detailed feedback.
Zoom Meeting Scheduler: 📅 Automatically schedule interviews with selected candidates.




