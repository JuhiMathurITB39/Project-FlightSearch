# Project-FlightSearch

# Flight Search Price Notifier ✈️  

## Overview  
An automated flight price tracking system that finds the cheapest flights using the Amadeus API and sends notifications via Twilio (SMS/WhatsApp) and Email.  

## Features  
✅ Retrieves the latest flight prices from Amadeus API  
✅ Updates Google Sheets with IATA codes  
✅ Sends WhatsApp, SMS, and Email alerts when prices drop  
✅ Secured with `.env` variables for sensitive data  

## Tech Stack  
- Python (Automation, API Handling)  
- Selenium & Requests (Web Scraping & API Calls)  
- Twilio API (SMS & WhatsApp Notifications)  
- Amadeus API (Flight Price Data)  
- Google Sheets API (Data Management)  

## Installation & Setup  
1️⃣ Clone the repository:  
git clone https://github.com/your-username/Flight-Search-Notifier.git
cd Flight-Search-Notifier
2️⃣ Install dependencies:
pip install -r requirements.txt
3️⃣ Create a .env file in the project folder with:
SHEETY_USERNAME=your_username
SHEETY_PASSWORD=your_password
SHEETY_PRICES_ENDPOINT=your_prices_sheet_endpoint
SHEETY_USERS_ENDPOINT=your_users_sheet_endpoint
AMADEUS_API_KEY=your_amadeus_api_key
AMADEUS_SECRET=your_amadeus_secret
TWILIO_SID=your_twilio_sid
TWILIO_AUTH_TOKEN=your_twilio_auth_token
TWILIO_VIRTUAL_NUMBER=your_twilio_number
TWILIO_VERIFIED_NUMBER=your_verified_number
MY_EMAIL=your_email
MY_EMAIL_PASSWORD=your_email_password

4️⃣ Run the script:
python main.py
How It Works
📌 1. Retrieves Destination Data → Gets flight destinations & updates IATA codes in Google Sheets
📌 2. Searches for Cheap Flights → Uses Amadeus API to find the lowest flight prices
📌 3. Sends Alerts → Notifies users via WhatsApp, SMS, and email if a price drop is found
