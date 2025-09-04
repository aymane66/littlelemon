# LittleLemon Reastaurant API

A RESTful API built with Django REST Framework for managing a restaurant's **menu items** and **table bookings**.  
This project demonstrates API design, authentication, permissions, and database modeling — suitable for portfolio presentation.

---

## Features
- **Menu Management**  
  - List, create, update, and delete menu items  
- **Booking Management**  
  - Book tables with guest count and reservation date  
  - CRUD operations via API  
- **Authentication**  
  - Token-based authentication using **Djoser** + DRF  
  - Session authentication for browsing via the DRF UI  
- **Permissions**  
  - Public users → read-only access to menu  
  - Authenticated users → full CRUD access to menu & bookings  

---

## Tech Stack
- **Backend:** Django 4.2, Django REST Framework
- **Authentication:** Djoser (Token Auth)
- **Database:** SQLite (default) or MySQL
- **Serialization:** DRF ModelSerializers
- **Extra Renderers:** JSON, Browsable API, XML

---

## API Endpoints

### Authentication
- `POST /auth/users/` → Register new user  
- `POST /auth/token/login/` → Get auth token  
- `POST /api-token-auth/` → Get token (DRF built-in)  

### Menu
- `GET /api/v1/menu/` → List all menu items  
- `POST /api/v1/menu/` → Add a new menu item *(auth required)*  
- `GET /api/v1/menu/<id>/` → Retrieve single menu item  
- `PUT /api/v1/menu/<id>/` → Update menu item *(auth required)*  
- `DELETE /api/v1/menu/<id>/` → Delete menu item *(auth required)*  

### Booking
- `GET /api/v1/booking/` → List all bookings *(auth required)*  
- `POST /api/v1/booking/` → Create a booking *(auth required)*  
- `GET /api/v1/booking/<id>/` → Retrieve booking *(auth required)*  
- `PUT /api/v1/booking/<id>/` → Update booking *(auth required)*  
- `DELETE /api/v1/booking/<id>/` → Cancel booking *(auth required)*  

---

## Installation & Setup

1. **Clone the repo**
```bash
  git clone https://github.com/yourusername/littlelemon-api.git
  cd littlelemon-api
```

2. **Create virtual environment**
```bash
python3 -m venv env
```

```bash
source venv/bin/activate   # macOS/Linux
venv\Scripts\activate      # Windows
```


3. **Install dependencies**
```bash
pip install -r requirements.txt
```

4. **Run migrations**
```bash
python3 manage.py migrate
```

5. **Start the server**
```bash
python3 manage.py runserver
```