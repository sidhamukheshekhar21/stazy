# 🏠 Stazy - Stay Easy
**AI-Powered Room Finder for Students**

---

## 📋 Project Overview
Stazy is a full-stack room finder platform built exclusively for students. It features AI-powered identity verification, fake listing detection, and seamless room booking near college campuses.

**Tech Stack:**
- Frontend: React.js
- Backend: Java Spring Boot
- Database: PostgreSQL
- Auth: JWT + OTP-based authentication
- Media: Cloudinary
- Migrations: Flyway

---

## 🚀 Getting Started

### Prerequisites
- Node.js v16+
- Java 17+
- Maven 3.8+
- PostgreSQL 14+

### Backend Setup
```bash
cd backend/backend

# Set environment variables
export STAZY_DB_URL=jdbc:postgresql://localhost:5432/stazy_db
export STAZY_DB_USERNAME=your_db_user
export STAZY_DB_PASSWORD=your_db_password
export STAZY_JWT_SECRET=your_jwt_secret

# Run
mvn spring-boot:run
```
Backend runs at `http://localhost:8080`

### Frontend Setup
```bash
cd frontend
npm install
npm start
```
Frontend runs at `http://localhost:3000`

---

## 📁 Project Structure
```
stazy/
├── backend/backend/
│   ├── src/main/java/com/stazy/backend/
│   │   ├── admin/        # Admin controllers, services, DTOs
│   │   ├── auth/         # JWT + OTP authentication
│   │   ├── booking/      # Booking & stay management
│   │   ├── complaint/    # Complaint system
│   │   ├── listing/      # Room listings
│   │   ├── profile/      # Student, Owner, Admin profiles
│   │   ├── security/     # Spring Security config
│   │   ├── user/         # User management
│   │   └── verification/ # AI-based verification
│   └── src/main/resources/
│       ├── application.yml
│       └── db/migration/ # Flyway SQL migrations
│
└── frontend/
    └── src/
        ├── components/shared/
        ├── pages/
        ├── services/     # API calls
        ├── utils/
        └── constants/
```

---

## 🎯 Pages

| Page | Description |
|------|-------------|
| Home | Landing page with hero, search, featured rooms |
| Explore Rooms | Filterable room listing |
| Login / Signup | Student & Owner auth with OTP |
| Student Dashboard | Bookings, profile, verification |
| Owner Dashboard | Listing management, booking requests |
| Admin Dashboard | Moderation, user management, analytics |
| Super Admin Dashboard | Platform-wide controls |

---

## 🔑 Environment Variables

| Variable | Description |
|----------|-------------|
| `STAZY_DB_URL` | PostgreSQL connection URL |
| `STAZY_DB_USERNAME` | DB username |
| `STAZY_DB_PASSWORD` | DB password |
| `STAZY_JWT_SECRET` | JWT signing secret |
| `CLOUDINARY_CLOUD_NAME` | Cloudinary cloud name |
| `CLOUDINARY_API_KEY` | Cloudinary API key |
| `CLOUDINARY_API_SECRET` | Cloudinary API secret |
| `STAZY_MAIL_HOST` | SMTP host |
| `STAZY_MAIL_PORT` | SMTP port |

---

## 🤖 AI Features
- Student identity verification via ID card photo
- Owner PAN card verification
- Fake listing detection from listing images

---

## 🚢 Deployment
- Frontend → Vercel / Netlify
- Backend → Railway / Render
- Database → Railway PostgreSQL / Supabase

---

*Built with ❤️ by the Stazy Team*
