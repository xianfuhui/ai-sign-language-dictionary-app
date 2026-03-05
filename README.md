# AI Sign Language Dictionary App

## Introduction

The **AI Sign Language Dictionary App** is a web-based application
designed to support learning, translation, and recognition of sign
language gestures.\
The system allows users to search for sign language meanings and explore
gesture-based communication through an interactive interface.

The application integrates **Artificial Intelligence** to recognize hand
gestures and translate them into corresponding meanings. This helps
improve accessibility and communication for learners interested in sign
language.

The platform provides both **learning and reference tools**, enabling
users to understand gestures quickly while practicing sign language in a
structured way.

------------------------------------------------------------------------

## Technologies Used

**Backend** - Node.js

**Frontend** - JavaScript - HTML - CSS

**Database** - MongoDB

------------------------------------------------------------------------

## Features

## Features

| No. | Category | Functionality |
|----|----------|---------------|
| 1 | Admin | Log in to the account |
| 2 | Admin | Log out of the account |
| 3 | Admin | View profile information |
| 4 | Admin | Edit profile |
| 5 | User Management | View user list |
| 6 | User Management | Change user status (locked users cannot access the system) |
| 7 | User | Register an account |
| 8 | User | Email verification required after registration |
| 9 | User | Log in to the account |
| 10 | User | Log out of the account |
| 11 | User | Forgot password |
| 12 | User | View profile information |
| 13 | User | Edit profile information |
| 17 | Admin | View all vocabulary list |
| 18 | Admin | Search vocabulary by letters |
| 19 | Admin | View vocabulary details |
| 20 | Admin | Add vocabulary |
| 21 | Admin | Edit vocabulary |
| 22 | Admin | Delete vocabulary |
| 23 | Admin | View suggested vocabulary list |
| 24 | Admin | Change status of suggested vocabulary |
| 25 | User | View all vocabulary list |
| 26 | User | View all letters list |
| 27 | User | View all difficulty levels list |
| 28 | User | Filter vocabulary by letter |
| 29 | User | Filter vocabulary by difficulty level |
| 30 | User | Search vocabulary by letters |
| 31 | User | View vocabulary details |
| 32 | User | Add vocabulary to favorites |
| 33 | User | View favorite vocabulary list |
| 34 | User | View practice vocabulary list |
| 35 | User | Practice with mock exams |
| 36 | User | View suggested vocabulary list |
| 37 | User | Suggest vocabulary |
| 38 | Admin | View all topics list |
| 39 | Admin | Search topics |
| 40 | Admin | View topic details and vocabulary within topics |
| 41 | Admin | Add topic |
| 42 | Admin | Edit topic |
| 43 | Admin | Delete topic |
| 44 | User | View all topics list |
| 45 | User | View topic details and vocabulary within topics |
| 46 | Admin | Train AI model for hand gestures |
| 47 | Admin | Upload AI model for hand gestures |
| 48 | Admin | Check if a video contains sign language |
| 49 | User | Use AI to guess vocabulary |
| 50 | User | Practice vocabulary using AI |
| 51 | User | Check if a video contains sign language |
| 52 | Admin | View total number of topics |
| 53 | Admin | View total number of users |
| 54 | Admin | View total number of vocabulary |
| 55 | Admin | View total number of favorite vocabulary |

------------------------------------------------------------------------

## Screenshots

### User Page

![User](docs/images/user.png)

### Gesture Recognition

![Feature](docs/images/ai.png)

### Admin Page

![Admin](docs/images/admin.png)

------------------------------------------------------------------------

## Local Deployment (Offline)

### Requirements

-   Node.js
-   MongoDB Compass

### Step 1 -- Download Project

Download and extract the application files to your local machine.

### Step 2 -- Configure Environment Variables

Example `.env` configuration:

    MONGO_URI=mongodb://127.0.0.1:27017/system
    PORT=3000
    KEY=your_secret_key
    USER_EMAIL=your_email
    PASS_EMAIL=your_email_password

Explanation:

-   **MONGO_URI**: MongoDB connection string to the local database.
-   **PORT**: Application running port (default: 3000).
-   **KEY**: Secret key used for application security.
-   **USER_EMAIL / PASS_EMAIL**: Email credentials used for
    account-related features.

### Step 3 -- Install Dependencies

    npm install

### Step 4 -- Start Application

    npm start

### Step 5 -- Import Database

Open **MongoDB Compass** and import JSON files from the
`source/Database` folder into the database **system**.

### Step 6 -- Access the Application

Admin site: http://localhost:3000/admin/login

Default admin account: Username: admin\
Password: admin

User site: http://localhost:3000/user

------------------------------------------------------------------------

## Production Deployment (Online)

### Required Platforms

-   GitHub: https://github.com/
-   Render: https://render.com/
-   MongoDB Atlas: https://www.mongodb.com/

### Deployment Steps

1.  Go to **MongoDB Atlas → Database Access** and create a database
    user.
2.  Go to **Network Access** and allow network access.
3.  Open **Database → Browse Collections**.
4.  Insert data from the **Database** folder.
5.  Click **Connect**.
6.  Choose **Drivers**.
7.  Copy the MongoDB connection string.
8.  Replace the `MONGO_URI` value in the `.env` file with the Atlas
    connection string.
9.  Push the source code to **GitHub**.
10. Go to **Render** and select **Deploy a Web Service**.
11. Select the repository containing the project.
12. Configure deployment settings.
13. Deploy the web service.
14. Verify the website after deployment.

------------------------------------------------------------------------

## Author

Name: Tien Phu Huy\
Email: tphuyvvk@gmail.com\
GitHub: https://github.com/xianfuhui
