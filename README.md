# DevInnovators-Open-Forum-Platform
A full-stack community forum platform built with HTML, CSS, JavaScript, and Express.js (Node.js). This project is designed for collaborative open source development, simulating real-world industry practices to help you learn version control, web development fundamentals, and teamwork.


folder structure :
open-forum-platform/
├── server.js                     # Main Express.js server file
├── package.json                   # Project dependencies
├── .env                           # Environment variables (DB credentials, API keys)
├── /public                        # Static assets (CSS, JavaScript, images)
│   ├── css/
│   │   └── styles.css             # Global styles (Tailwind can be used)
│   ├── js/
│   │   └── app.js                 # Client-side JavaScript (e.g., navbar interactions)
│   └── images/                    # Image assets
├── /routes                        # Express.js route handlers (API Endpoints)
│   ├── about.js                   # Team 1 - About / Mission Page
│   ├── dashboard.js               # Team 2 - Forum Overview
│   ├── notifications.js           # Team 3 - Notifications
│   ├── settings.js                # Team 4 - Settings
│   ├── help.js                    # Team 5 - Help / FAQ
│   ├── search.js                  # Team 6 - Search
│   ├── admin.js                   # Team 7 - Admin Dashboard
│   ├── categories.js              # Team 8 - Categories / Threads Listing
│   ├── profile.js                 # Team 9 - User Profile
│   ├── thread.js                  # Team 10 - Thread Details (Dynamic)
│   ├── new-thread.js              # Team 11 - New Thread
│   ├── auth.js                    # Team 12 & 13 - Login & Registration
│   ├── index.js                   # Team 14 - Home Page API
│   └── router.js                  # Main router to combine all routes
├── /views                         # **Now contains static HTML instead of EJS**
│   ├── about.html                 # About Page
│   ├── dashboard.html              # Forum Overview
│   ├── notifications.html          # Notifications Page
│   ├── settings.html               # Account Management
│   ├── help.html                   # Help / FAQ
│   ├── search.html                 # Search Results
│   ├── admin.html                  # Admin Dashboard
│   ├── categories.html             # Categories Page
│   ├── profile.html                # User Profile
│   ├── thread.html                 # Thread Details (Dynamic)
│   ├── new-thread.html             # New Thread Creation
│   ├── login.html                  # Login Page
│   ├── register.html               # Registration Page
│   ├── index.html                   # Home Page
│   └── partials/                   # Partial components (e.g., navbar, footer)
│       ├── navbar.html              # Navbar
│       └── footer.html              # Footer
├── /controllers                   # Business logic for API routes
│   ├── authController.js           # Login & Registration logic
│   ├── threadController.js         # Threads handling
│   ├── userController.js           # User profile & settings
│   ├── adminController.js          # Admin panel logic
│   ├── categoryController.js       # Forum categories
│   └── homeController.js           # Homepage logic
├── /models                        # Database models (PostgreSQL using Sequelize or pg)
│   ├── User.js                     # User model
│   ├── Thread.js                   # Forum threads model
│   ├── Category.js                 # Categories model
│   ├── Comment.js                  # Comments on threads
│   └── index.js                     # DB connection setup
├── /config                        # Configurations
│   ├── database.js                 # PostgreSQL connection
│   ├── auth.js                     # Authentication config (JWT, sessions)
│   ├── passport.js                 # Passport.js strategy (if using auth)
│   └── middleware.js                # Middleware functions
├── /migrations                    # Database migration files (if using Sequelize)
│   ├── 001-create-users.js         # Example migration for users
│   ├── 002-create-threads.js       # Example migration for threads
│   ├── 003-create-comments.js      # Example migration for comments
│   └── 004-create-categories.js    # Example migration for categories
└── /seeds                         # Database seeding files
    ├── usersSeed.js                # Seed initial users
    ├── threadsSeed.js              # Seed initial threads
    ├── commentsSeed.js             # Seed initial comments
    └── categoriesSeed.js           # Seed initial categories