# 30 Days DevOps Challenge - Weather Dashboard

## Day 1: Building a Weather Data Collection System using AWS S3 and OpenWeather API

---

## Project Overview
This project is a **Weather Data Collection System** that showcases key DevOps principles. It integrates:
- **External API**: OpenWeather API for fetching weather data
- **Cloud Storage**: AWS S3 for secure and scalable data storage
- **Infrastructure as Code**
- **Version Control**: Using Git for collaboration and tracking
- **Python Development**: Clean, modular, and reusable code
- **Error Handling**: Resilience in distributed systems
- **Environment Management**: Secure handling of sensitive credentials

---

## Features
- Fetches **real-time weather data** for multiple cities.
- Displays:
  - Temperature (°F)
  - Humidity levels
  - General weather conditions.
- Automatically stores the data in **AWS S3** for future access.
- Tracks multiple cities with timestamps for historical reference.

---

## Technical Architecture
- **Programming Language**: Python 3.x
- **Cloud Provider**: AWS (S3)
- **External API**: OpenWeather API
- **Key Dependencies**:
  - `boto3`: AWS SDK for Python
  - `python-dotenv`: For managing environment variables
  - `requests`: For API integration

---

## Project Structure

weather-dashboard/ 
├── src/ 
    ├── init.py 
    └── weather_dashboard.py # Main logic for fetching and storing weather data 
├── .env # Environment variables (API keys, credentials)
├── .gitignore # Ignored files for version control 
├── requirements.txt # Python dependencies 
└── README.md # Project documentation



---

## Setup Instructions

### 1. Clone the Repository
```bash
git clone https://github.com/ShaeInTheCloud/30days-weather-dashboard.git
cd 30days-weather-dashboard
2. Install Dependencies

bash

pip install -r requirements.txt

3. Configure Environment Variables
Create a .env file in the root directory and add the following variables:
makefile

OPENWEATHER_API_KEY=your_openweather_api_key
AWS_BUCKET_NAME=your_s3_bucket_name

4. Configure AWS Credentials
Ensure your system is configured with AWS credentials:

bash

aws configure
Provide your AWS Access Key ID, Secret Access Key, and default region.

5. Run the Application
bash

python src/weather_dashboard.py

What I Learned

AWS S3: Creating and managing S3 buckets for cloud storage.
Environment Variables: Secure handling of sensitive API keys and credentials using .env files.
API Integration: Fetching data from external APIs with error handling.
Python Development: Applying best practices for reusable and modular code.
Git Workflow: Using Git for version control and collaboration.
Error Handling: Managing failures in distributed systems.
Cloud Resource Management: Deploying and integrating cloud-based services.

Feel free to explore, modify, and contribute to this project.
Happy coding!
