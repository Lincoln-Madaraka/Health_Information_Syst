# Health Information System

A Django-based Health Information System designed to help doctors manage health programs/services and client enrollment efficiently.

## 📌 Project Overview

This system allows a doctor (system user) to:

1. **Create health programs** – e.g., TB, Malaria, HIV, etc.
2. **Register new clients** into the system.
3. **Enroll clients** into one or more health programs.
4. **Search for clients** from a list of registered individuals.
5. **View client profiles**, including their enrolled programs.
6. **Expose client profiles via a REST API** for integration with external systems.

## 🏗️ Project Structure (Planned)

The project is organized into the following Django apps:

- `clients` – Handles client registration, search, and profile views.
- `programs` – Manages creation and listing of health programs.
- `enrollment` – Manages enrollment of clients into health programs.
- `api` – Provides API endpoints to expose client profiles.

## 🛠️ Features to Implement

| Feature                         | Status  |
| ------------------------------ | ------- |
| Create health program          | ✅ Done |
| Register new client            | ✅ Done |
| Enroll client in programs      | ✅ Done |
| Search for client              | ✅ Done |
| View client profile            | ✅ Done |
| REST API for client profile    | ✅ Done |

## 🧰 Technologies Used

- Python 3.x
- Django 4.x
- Django REST Framework
- SQLite (for local development)
- Bootstrap (for styling and layout)

## ⚙️ Setup Instructions

1. **Clone the repository:**
   ```bash
   git clone https://github.com/yourusername/Health_Information_Syst.git
   cd Health_Information_Syst

