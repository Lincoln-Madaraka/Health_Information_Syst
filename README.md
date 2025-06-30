
# Health Information System

This project simulates a **basic Health Information System** where a doctor (system user) can:

- Create health programs (e.g., TB, Malaria, HIV, etc.)
- Register clients (patients)
- Enroll clients into one or multiple programs
- Search for registered clients
- View a client's profile and enrolled programs
- Expose client profiles through a simple **REST API**

> Developed as part of the **CEMA Software Engineering Internship Application Task**.

The project was deployed to render: [Deployed System](https://health-information-syst.onrender.com/) Login Username: admin Password: admin
Powerpoint Slides: [View Slides](https://docs.google.com/presentation/d/1t-d_yXyOhkNgrmw327xdixcqX81_9nBN0f4DIM-Gf1c/edit?usp=drivesdk)
Protype: [Watch Here](https://drive.google.com/file/d/1mxM-FePJjD4EieP43tuHWEX6jtkGLT1j/view?usp=drivesdk)

---

## Table of Contents
- [Project Structure](#project-structure)
- [Key Features](#key-features)
- [Technology Stack](#technology-stack)
- [Setup Instructions](#setup-instructions)
- [API Endpoints](#api-endpoints)
- [Prototype Demonstration](#prototype-demonstration)
- [Deployment](#deployment)
- [Future Improvements](#future-improvements)
- [Presentation and Demo](#presentation-and-demo)
- [Contact](#contact)

---

## Project Structure

The repository is organized as follows:

```bash
HealthInformationSystem/        # Main Django project folder
├── __init__.py
├── asgi.py
├── manage.py                   # Django management script
├── requirements.txt            # Project dependencies
├── settings.py                 # Django project settings
├── urls.py                     # Project URL configurations
├── wsgi.py
├── vercel.json                 # For deployment
health/                         # Main Django app for health system
├── __init__.py
├── admin.py                    # Django admin customization
├── apps.py
├── migrations/                 # Database migration files
├── models.py                   # Database models (Program, Patient, Appointment)
├── static/                     # Static assets (CSS, JS)
├── templates/                  # HTML templates for views
├── tests.py                    # Unit tests (basic)
├── views.py                    # Core application logic
db.sqlite3                      # SQLite database
staticfiles/                    # Collected static files for deployment
docs/                           # Documentation folder
├── Presentation.pptx           # PowerPoint Presentation
├── Prototype_Demo_Video.mp4     # Prototype Demonstration Video
Procfile                        # For Render deployment
venv/                           # Python virtual environment (not pushed to GitHub)
```

---

## Key Features

✅ Create health programs like HIV, TB, Malaria  
✅ Register new clients into the system  
✅ Enroll clients into one or more programs  
✅ View client profiles with their enrolled programs  
✅ Search for registered clients by name  
✅ Expose client profile data via a simple public **API**  
✅ Clean and documented code  
✅ Project deployed publicly on Render  
✅ Simple and intuitive frontend (HTML/CSS + minimal JavaScript)

---

## Technology Stack

- **Backend Framework:** Django (Python)
- **Frontend:** HTML, CSS, Bootstrap
- **Database:** SQLite (default Django setup)
- **Deployment:** Render
- **API:** Django REST framework (simple implementation)

---

## Setup Instructions

🔹 To run the project locally:

1. **Clone the repository**

```bash
git clone https://github.com/YOUR_USERNAME/HealthInformationSystem.git
cd HealthInformationSystem
```

2. **Create a virtual environment and activate it**

```bash
python3 -m venv venv
source venv/bin/activate   # For Linux/macOS
venv\Scripts\activate      # For Windows
```

3. **Install the dependencies**

```bash
pip install -r requirements.txt
```

4. **Run migrations**

```bash
python manage.py makemigrations
python manage.py migrate
```

5. **Create a superuser (admin login)**

```bash
python manage.py createsuperuser
```

6. **Start the development server**

```bash
python manage.py runserver
```

7. **Access the app**
- Visit `http://127.0.0.1:8000/` on your browser.

---

## API Endpoints

🔹 A simple API is exposed to retrieve client profiles.

| Endpoint | Description |
|:---|:---|
| `/api/clients/` | Returns a list of all registered clients and their enrolled programs in JSON format |

Example Output:
```json
[
  {
    "id": 1,
    "name": "John Doe",
    "programs": ["HIV Program", "Malaria Program"]
  },
  ...
]
```

> 🔥 **API-first Approach:** The API is designed to be easily extendable for future systems integration.

---

## Prototype Demonstration

You can view the working prototype demo through:

- 📽️ **Prototype Demo Video:**  
[Watch Here](https://drive.google.com/file/d/1mxM-FePJjD4EieP43tuHWEX6jtkGLT1j/view?usp=drivesdk)

- 🖼️ **PowerPoint Presentation:**  
[View Slides](https://docs.google.com/presentation/d/1t-d_yXyOhkNgrmw327xdixcqX81_9nBN0f4DIM-Gf1c/edit?usp=drivesdk)

Both the presentation and the video are also available in the `docs/` folder in the repository.

---

## Deployment

The project is deployed on **Render** for easy access.  

Deployment steps:
1. Pushed to GitHub.
2. Connected GitHub repository to Render.
3. Configured **Procfile** and **vercel.json**.
4. Automatic deploy on `git push`.

---

## Future Improvements

- Add unit tests for all major models and views.
- Improve the API (pagination, authentication).
- Add detailed client histories and appointment scheduling.
- Implement security features (user authentication, access roles).
- Optimize database queries and indexes for large datasets.
- Deploy using a production-grade database like PostgreSQL.

---

## Presentation and Demo

| Material | Link |
|:---|:---|
| PowerPoint Presentation | [View Here](https://docs.google.com/presentation/d/1t-d_yXyOhkNgrmw327xdixcqX81_9nBN0f4DIM-Gf1c/edit?usp=drivesdk) |
| Prototype Demonstration Video | [View Here](https://drive.google.com/file/d/1mxM-FePJjD4EieP43tuHWEX6jtkGLT1j/view?usp=drivesdk) |

---

## Contact

> Developed by **Lincoln Madaraka**

- 📧 Email: madarakalincoln48@gmail.com
- 🌐 Portfolio: [Lincoln Madaraka Portfolio](https://lincoln-madaraka-portfolio.vercel.app/)

---

# Thank you for reviewing this project! 🚀 Optimization coming up soon

