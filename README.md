# Buy-Sell Marketplace (Bazaar)

## Overview
Full-stack buy-sell marketplace application with user authentication, product listings, cart, checkout, and order management. Built with React frontend, Node.js/Express backend, Prisma + PostgreSQL.

## Features
### User Management
- Registration and Login with JWT authentication
- Profile management
- Protected routes

### Seller Features
- Create product listings (single or bulk via CSV/JSON)
- Upload images
- Manage listings (update, set active/inactive)
- View sales reports

### Buyer Features
- Browse marketplace
- Search and apply filters
- View product details
- Add to cart
- Cart management
- Checkout with address selection and Razorpay payment
- Order confirmation

### Additional
- Guest browsing
- Responsive UI
- Real-time toast notifications
- Docker support

## Tech Stack
- **Frontend**: React, Vite, React Router
- **Backend**: Node.js, Express, Prisma ORM
- **Database**: PostgreSQL
- **Auth**: JWT + bcrypt
- **Payments**: Razorpay
- **Email**: Nodemailer
- **Deployment**: Docker Compose

## Architecture
[![](https://mermaid.ink/img/pako:eNqtV0tv4jAQ_iuRpb1BVVKghVuXqhL7alXay4qLGw9g1bGztlNKgf--4yS0CThagjYHRDyfx_P4ZsZZk0gxIEMC-obTuabxVE9lgM-TAR2sd2_umVjN5TzgLLj_7lmfcW3sLxqDRyZorQhiykXw5NOYUGOWSrOy6EEJCDT--PBazbiAcUznFfENtfDIYwgiDfiXXduddOv-7F6uGdNgTCOnU4zSmAW33oCkQtQ4nSyU9K0bqwGsRxBxu_Li0R-ffoUSMcLU-nSpVFpdUfdVYUSpDLi5gRlNhT0hfD-4sU59k_BZbr2ZZGAizRPLlfRInzWVFVLcCkUtpp9HFWUjJRl3OtDl4p_PaQlzZTl9rlryzeA-S-fGH6eJEswvuY4sf_Xzj4GASgDdM5YW86iiF19-QYh6gkWod6706kB-ZMZGxf5GKZPI6FK5VhRmldesfrTwtYucShW_KgfdadawOz2nq_pA-s4riWneGA7EOe2swlK73-deZuEEyzM1WZWm5oQE3dNVDEiPoxzNraGxq-7yeqGk1pZCXwx2oZhHoJwnme_BlGDiyUlM0_a0vtrozIo0Tdg_LBpbiBtZFblNDTnkyvtPSqXd6-ClnjWRNDELZf-7kw_wymF5nIvOTk2dC96RETsONRyAdSE5kjR3NnlULyCr9js76_KT3SV8Y8ap8VoAbwnH2q5Gd9fL0Td2gt1fvmDgBXXjxix4Yio3qs2m3Vbrj7vGEPm9oOaT4GXQbqI6kJsENbC8GToQNrkaTMEEB1pqbsEH22zyOnUgtZQF5GBYeIwrBhF_L-vdvxcU-_IZke1S0lIuS1v2oCWjNUSAU7Ue-xmEJNURhhRYwGUt_KP83Q7s74imBw5jLHzwqt37t8cDexwHkuJSgyZkvDiMUo4v0rDr-5k7FNn-yumUkBaZa87I0OoUWiQGjXTHV7J2KqbELgAvmyQPF0vf2ozql3akhNJ4ntzi_oTK30rFOxVapfMFGc6oMPiW95LiM-BjVYNEy0ZuqpBhP-xnSshwTd7IsBP2z8JBJ-x2umG_N-j0LlpkRYbtTv_8rHc16Ia9znnYuTjvhdsWec8O7px1LweXuHKJ-O4Vbm0RwLuZ0j_zD5Hse2T7F-RC59c?type=png)](https://mermaid.live/edit#pako:eNqtV0tv4jAQ_iuRpb1BxauUcutSVWJfrUp7WXFx4yFYdeys7ZRSyn_fcRLaBBwtQZtDlGQ-j-fxzYyzIaFiQMYE9DWnkabxXM9lgNejAR1sdm_umlnNZRRwFtx993xfcG3sLxqDRyZorQhiykXw6NOYUGNWSrOy6F4JCDTefHitFlzANKZRRXxNLTzwGIJQAz6yK7uTbt3D7uWKMQ3GNHI6xShNWXDjDUgqRI3TyVJJ33djNYD1CEJu1148-uPTr1AiJphany6VSqsr6r4qjCiVATfXsKCpsCeE7wc31qlvEj7LrTeTDEyoeWK5kh7pk6ayQooboajF9POwomyiJONOB7pcPPmclhApy-lT1ZJvBtdZGhl_nGZKML_kKrT8xc8_BgIqAXTXVFrMowqfffkFIeoJFqLeSOn1gfzIjE2K9Y1SJpHRpXKtKMwqr1n9aOFrFzmVKn5VNrrVrGF3ekrX9YH07VcS07wxHIhz2lmFpXa3z73MwhmWZ2qyKk3NCQm6o-sYkB5HOZpbQ2NX3eXvhZJaWwp9MdilYh6Bcp5kvgdzgoknJzFN29P6aqM9K9I0Yf-waGohbmRV6BY15JAr7z8plXavg5d61kzSxCyV_e9O3sMLh9VxLjo7NXUueEdG7DjUcADWheRI0tza5EE9g6za7-ysy092lvCNGafGawG8JhxruxrdXS9H39gJdn_5goEX1I0bs-SJqZyo3t_bbbX5OGuMkd9Laj4JXgbtJqoDuUlQA8uboQNhk6vBFExwoJXmFnyw9_e8Th1IrWQBORgWHuOKQcTfynr3zwXFunxGZKuUtJTL0pI9aMloDSHgVK3HfgYhSXWIIQUWcFkL_yh_twL7O6LpgcMYCx-8avf-6fHAHseBpDjUoAkZLw6jlOOLNOz6fuYORba_cDonpEUizRkZW51Ci8Sgke74SjZOxZzYJeBhk-ThYulrm1H93A6VUBr3k1tcn1D5W6l4p0KrNFqS8YIKg295Lyl-Az6-apBo2cRNFTIedkeZEjLekFcy7nc6Z73eaNTrDTqjQX-IwjUZt0dn_c6o373sdga9i0Hv8mLbIm_Ztp2z0WjYPR_2L8673c5lfzhoEcCTmdI_89-Q7G9k-xcgJOeA)
## Setup (Docker)
1. Clone the repository
2. Copy provided `docker-compose.yml`, server Dockerfile, etc.
3. Update environment variables in `docker-compose.yml` (DB credentials, JWT secret, Razorpay keys, email)
4. Run: `docker-compose up --build`
5. Access:
   - Client: http://localhost:5173
   - Server: http://localhost:4000
   - DB: localhost:5432

## Manual Setup
- Backend: `cd server && npm install && npx prisma migrate dev && npm run dev`
- Frontend: `cd client && npm install && npm run dev`

## API Routes
- `/api/auth` - Auth endpoints
- `/api/listings` - Product listings
- `/api/cart` - Cart operations
- `/api/orders` - Orders and checkout
- `/api/addresses` - User addresses

## Project Structure
- `/client`: React app
- `/server`: Node/Express backend with Prisma

## Environment Variables
See `docker-compose.yml` for keys: DATABASE_URL, JWT_SECRET, RAZORPAY keys, MAIL credentials.

## Screenshots / Diagrams
[Workflow Image](buy-sell-workflow.png)
