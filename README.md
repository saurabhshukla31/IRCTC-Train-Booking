IRCTC Train Booking Automation
A Cypress-based automation script for booking IRCTC Tatkal tickets in under a minute by automating the login, captcha solving, and multiple passenger details filling process.

Features
Book Tatkal, Premium Tatkal, and Normal Tickets.
Auto-login with your IRCTC username and password.
Captcha solving and retry mechanism for increased success.
Multiple passenger support with pre-filled information.
UPI ID or QR Code for payment gateway automation.
Supports food choices, seat preferences, and auto-upgradation.
Books only when confirmed berths are available.
Setup
Install NodeJS, Python, and pip.
Clone the repository:
bash
Copy code
git clone https://github.com/saurabhshukla31/IRCTC-Train-Booking.git
Configure passenger details in cypress/fixtures/passenger_data.json.
Set your IRCTC login credentials in cypress.env.json.
Install required dependencies:
bash
Copy code
npm install
pip install -r irctc-captcha-solver/requirements.txt
Run the automation:
bash
Copy code
npx cypress run --headed --no-exit
Configuration
Edit cypress/fixtures/passenger_data.json to update your:

Train number, class, date, source, and destination.
Passenger details: name, age, gender, seat preference, and food choice.
Edit cypress.env.json for IRCTC login credentials and captcha mode:

json
Copy code
{
    "USERNAME": "yourusername",
    "PASSWORD": "yourpassword",
    "MANUAL_CAPTCHA": false
}
Tip: Set MANUAL_CAPTCHA to true if you want to enter the captcha manually.

Disclaimer
This project is for educational purposes only. The author is not responsible for any misuse of this code that violates IRCTC’s terms of service.

