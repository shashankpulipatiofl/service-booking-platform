# Service Booking Platform (Home Lynk)

A role-based full-stack web application that enables users to book home services, service providers to manage assigned work, and administrators to control operations efficiently.

---

## Overview

This project simplifies home service booking and management through a unified platform supporting customers, service professionals, and administrators.

---

## Highlights

- Role-based architecture (User, Provider, Admin)
- End-to-end booking workflow (cart → checkout → order tracking)
- Automatic job assignment based on provider workload
- Commission-based revenue model

---

## Key Features

### User
- Browse service categories  
- Add services to cart  
- Select time slot, address, and payment method  
- Place and track bookings  

### Provider
- Register and complete profile verification  
- Upload required documents  
- View assigned jobs  
- Update work status  

### Admin
- Approve or reject provider profiles  
- Assign bookings (manual/automatic)  
- Monitor orders and payouts  
- Manage commission distribution  

---

## Tech Stack

| Layer | Technology |
|------|-----------|
| Backend | Python (Flask) |
| Database | MySQL |
| ORM | Flask-SQLAlchemy |
| Frontend | HTML, CSS, JavaScript |
| Templating | Jinja2 |

---

## Project Structure

```bash
service-booking-platform/
│── app.py
│── schema.sql
│── README.md
│── PROJECT_GUIDE.md
│
├── templates/
├── static/
```

---

## Installation and Setup

### 1. Clone the repository
```bash
git clone https://github.com/shashankpulipatiofl/service-booking-platform.git
cd service-booking-platform
```

### 2. Install dependencies
```bash
pip install flask flask-sqlalchemy pymysql werkzeug
```

### 3. Configure database
- Create a MySQL database  
- Import schema:

```bash
mysql -u root -p < schema.sql
```

### 4. Run the application
```bash
python app.py
```

### 5. Access the application
```
http://127.0.0.1:5000/
```

---

## Core Logic

- Automatic assignment of professionals based on availability and workload  
- Validation to ensure one service category per booking  
- Commission split: 20% admin, 80% provider  
- Role-based access control  

---

## Security

- Password hashing using Werkzeug  
- Role-based access control  
- Restricted access to uploaded documents  

---

## Limitations

- No payment gateway integration  
- Hardcoded configuration values  
- Monolithic backend  

---

## Future Enhancements

- Payment integration  
- Email/OTP verification  
- Notification system  
- Cloud deployment  
- Modular backend using Flask Blueprints  

---

## Author

Shashank Pulipati  

---

## License

This project is for educational purposes.
