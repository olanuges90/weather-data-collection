# Real-Time Weather Data Collection - Day 1 AllStarsDevOps Challenge

![image](https://github.com/user-attachments/assets/e65dc8b1-abb0-4d0f-8dc6-1b3c78d69369)


# Project Overiew
In this Project, I will build a Python Application that fetches real-time weather data from the OpenWeather API and the collected data will be securely stored in AWS S3 Bucket.

This Project demonstrates Core DevOps principles by highlighting the following Features:
- External API Integration (Real-time Data from the OpenWeather API)
- AWS Cloud Storage (S3 Buckets)
- Git for version Control
- Python Development
- Error Handling
- Environmental Management
- Troubelshooting (A must for DevOps}
- Documentation
# Features
- Fetches real-time weather data for multiple cities
- Displays temperature (°F), humidity, and weather conditions
- Automatically stores weather data in AWS S3
- Supports multiple cities tracking
- Timestamps all data for historical tracking
# Prerequisities
- Python 3.8+ Installed
- An OpenWeather API Key (OpenWeather API)
- AWS User Account with S3 Permissions
# Dependencies
- boto3
- python-dotenv
- requests
# Project Structure

    weather-dashboard/
     src/
      __init__.py/
      weather_dashboard.py
     tests/
     data/
     .env
     .gitignore
     requirements.txt
     
# Project Setup and Installation 
1. Clone the repository
     
         git clone https://github.com/olanuges90/weather-data-collection.git
     
2. Set up Python virtual environment

         python -m venv venv

         source venv/bin/activate  #To activate the virtual enevironment
   
3. Install dependencies

         pip3 install -r requirements.txt

4. Create environment (.env) variables in the root directory to store API Key securely

        OPENWEATHER_API_KEY=your_api_key
        AWS_BUCKET_NAME=your_bucket_name

5. Configure AWS Credentials

       aws configure
   
6. Add Environment variables and AWS credentials to .env

       echo "OPENWEATHER_API_KEY=your_api_key" >> .env
       echo "AWS_BUCKET_NAME=<your_bucket_name" .env
       echo "AWS_ACCESS_KEY_ID=your_access_key" >> .env
       echo "AWS_SECRET_ACCESS_KEY=your_secret_key" >> .env
       echo "AWS_DEFAULT_REGION=your_region" >> .env
   
8. Run the application

       python3 src/weather_dashboard.py
# Future Enhancements
- Dockerize the applicaton
- Setup CI/CD pipelines using Github Actions
- Schedule daya collection with cron jobs or AWS Lambda
- Add more units to improve test coverage
