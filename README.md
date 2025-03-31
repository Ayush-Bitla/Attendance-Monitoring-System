# Attendance Monitoring System

## Overview
The **Attendance Monitoring System** is a project designed to streamline and automate attendance tracking using a fingerprint-based authentication system. This system eliminates manual attendance marking, reducing errors and improving efficiency.

## Features
- Biometric fingerprint authentication for secure and accurate attendance marking
- Real-time data recording and storage
- User-friendly interface for students and administrators
- Automated attendance reports generation
- Secure database management

## Technology Stack
- **Hardware:** ESP-12F, Fingerprint Sensor
- **Software:** Django (Python), Embedded C
- **Database:** MySQL
- **Tools & Frameworks:** Arduino IDE, Proteus for circuit simulation, Django Framework

## Installation & Setup
1. Clone the repository:
   ```sh
   git clone https://github.com/Ayush-Bitla/Attendance-Monitoring-System.git
   ```
2. Install required dependencies:
   - Ensure you have **Arduino IDE** installed for microcontroller programming.
   - Install MySQL for database management.
   - Set up a **Django virtual environment**:
     ```sh
     python -m venv venv
     source venv/bin/activate  # For Mac/Linux
     venv\Scripts\activate  # For Windows
     ```
   - Install required Python dependencies:
     ```sh
     pip install -r requirements.txt
     ```
3. Upload the firmware to the ESP8266 microcontroller using Arduino IDE.
4. Apply Django migrations:
   ```sh
   python manage.py migrate
   ```
5. Create a superuser (optional, for admin access):
   ```sh
   python manage.py createsuperuser
   ```
6. Run the Django backend server:
   ```sh
   python manage.py runserver
   ```
7. Connect the fingerprint scanner and ensure proper communication with the ESP-12F.

## Usage
- Register fingerprints for new users through the admin panel.
- Users scan their fingerprints to mark attendance.
- Attendance records are stored in the database and can be retrieved for reporting.

## Future Enhancements
- Integration with cloud storage for remote access
- Mobile application for easier attendance tracking
- Facial recognition as an alternative authentication method

## License
This project is licensed under the [MIT License](LICENSE).
