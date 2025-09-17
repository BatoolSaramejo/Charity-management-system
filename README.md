# Charity Management System - Backend (Laravel API)

This project is a **Charity Management System** backend built with **Laravel**.  
It provides a complete set of APIs to manage **donations, beneficiaries, volunteers, admins, and super admins**, ensuring transparency and efficiency in charitable operations.

---

##  Features (Functional Requirements)

###  Donor
- Register, login, logout, reset password.
- Browse ongoing and urgent charity projects (health, education, housing, food).
- View completed projects and project details (amount needed, progress, status).
- Save favorite projects and search through them.
- Top-up wallet balance and donate directly from the wallet.
- Calculate and pay Zakat.
- View personal donation history.
- Receive notifications about project updates and status.
- Monthly auto-donation option (enable/disable anytime).
- Earn points for donations and appear in a "Top Donors" list.
- Send gifts (financial support) directly to beneficiaries.
- Submit volunteer requests via a questionnaire and track status.
- View and provide feedback on experiences.

###  Beneficiary
- Register, login, logout.
- Submit a help request through a structured form (health, education, housing, food).
- Track request status (under review, approved, rejected).
- Receive notifications about request progress.
- View percentage of donations collected for their request.
- Receive financial gifts and track delivery status.
- Provide feedback on their experience.

###  Volunteer
- Register, login, logout.
- Submit volunteer applications via a questionnaire.
- Track request status (under review, approved, rejected).
- Participate in one project at a time.
- Receive notifications about assignments and progress.

###  Admin
- Login, logout.
- View organization statistics (donations, beneficiaries, volunteers).
- Manage projects: add, update status (active, pending, finished), or delete.
- Assign donations from association’s balance to projects.
- Manage volunteer requests: review, approve/reject, ban/unban volunteers.
- Manage beneficiary requests: review, approve/reject, ban/unban beneficiaries.
- Manage donations and monthly contributions.
- Manage gifts: review delivery status and mark as delivered.
- Review and approve/reject feedback from beneficiaries.

###  Super Admin
- Login, logout.
- View statistics about completed projects.
- Manage admins: add new accounts, search, block/unblock.
- Review donation records of admins for transparency.


---

##  Tech Stack
- **Backend**: Laravel (PHP)
- **Database**: MySQL
- **Frontend Clients**: Flutter (Mobile & Web), React (Web Admin Panel)

---

##  Installation
1. Clone repository:
   ```bash
   git clone https://github.com/BatoolSaramejo/charity-backend.git
   cd charity-backend

2. Install dependencies:
    composer install

3. Copy environment file:
    cp .env.example .env

4. Set up .env (database, mail, etc.)

5. Generate app key:
    php artisan key:generate

6. Run migrations:
    php artisan migrate

7. Start server:
    php artisan serve


 ##   Project Structure

   - app/Models → Eloquent models

   - app/Http/Controllers → API controllers

   - routes/api.php → API routes

   - database/migrations → Database schema

   - config/ → Application configuration
   

 ## API Documentation (Basic)

   - POST /api/register → Register a new user

   - POST /api/login → User login

   - GET /api/projects → List active projects

   - POST /api/donate → Make a donation

   - POST /api/help-request → Submit a beneficiary help request

   - POST /api/volunteer-request → Submit volunteer application