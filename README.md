# 🚄 IRCTC Train Booking Automation

https://github.com/user-attachments/assets/2c6ff7ee-7cf5-49e2-a438-03d916d55293

A **Cypress-based automation script** to book IRCTC Tatkal tickets effortlessly in under a minute, automating login, captcha solving, and passenger details filling.

---

## ✨ Features

- ✅ Book **Tatkal**, **Premium Tatkal**, and **Normal Tickets**.
- ✅ Auto-login using **IRCTC credentials**.
- ✅ **Captcha solving** with retries for successful booking.
- ✅ Support for **multiple passengers** with pre-filled details.
- ✅ **Payment automation** via **UPI ID** or **QR Code**.
- ✅ Choose **food preferences** and **seat preferences**.
- ✅ **Auto-upgradation** enabled.
- ✅ Book only if **confirmed berths** are available.

---

## 🛠 Setup

### Prerequisites

- Install **NodeJS**, **Python**, and **pip**.

### Steps

1. **Clone the repository**:
   ```bash
   git clone https://github.com/saurabhshukla31/IRCTC-Train-Booking.git
   ```
2. **Configure passenger details** in `cypress/fixtures/passenger_data.json`.
3. **Set your IRCTC login credentials** in `cypress.env.json`.
4. **Install dependencies**:
   ```bash
   npm install
   pip install -r irctc-captcha-solver/requirements.txt
   ```
5. **Run the automation**:
   ```bash
   npx cypress run --headed --no-exit
   ```

---

## ⚙️ Configuration

### Passenger Details (`cypress/fixtures/passenger_data.json`)
- **TRAIN_NO**: Train number (e.g., `"12318"`).
- **TRAIN_COACH**: Coach class (e.g., `"3A"`).
- **TRAVEL_DATE**: Date of travel (e.g., `"12/09/2023"`).
- **SOURCE_STATION**: Source station (e.g., `"UMB"`).
- **DESTINATION_STATION**: Destination station (e.g., `"BSB"`).
- **PASSENGER_DETAILS**: Array of passenger details with:
  - `NAME`: Passenger name.
  - `AGE`: Passenger age.
  - `GENDER`: Male/Female/Transgender.
  - `SEAT`: Seat preference (e.g., `"Side Upper"`).
  - `FOOD`: Food preference (Veg/Non-Veg/No Food).

### IRCTC Credentials (`cypress.env.json`)
```json
{
    "USERNAME": "yourusername",
    "PASSWORD": "yourpassword",
    "MANUAL_CAPTCHA": false
}
```
> **Note**: Set `MANUAL_CAPTCHA` to `true` if you wish to manually enter captcha.

---

## ⚠️ Disclaimer

> **For educational purposes only**. The author takes no responsibility for any misuse that violates IRCTC's terms of service or legal implications.


