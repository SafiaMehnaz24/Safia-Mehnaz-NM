# Firebase Studio

This is a NextJS starter in Firebase Studio.

To get started, take a look at src/app/page.tsx.
# Job Application Tracker

## Project Overview

Job Application Tracker is a web application built to help job seekers organize, manage, and track their job applications. It provides a central dashboard to monitor application statuses, store important details like company information, job descriptions, contacts, and interview dates, streamlining the job search process and replacing the need for messy spreadsheets.

---

## Features

-   **Authentication:** Secure user sign-up and login, ensuring all application data is private.
-   **Dashboard View:** A clean, visual (Kanban-style) dashboard to see all applications at a glance.
-   **Status Tracking:** Easily categorize applications by status (e.g., "Wishlist", "Applied", "Interviewing", "Offer", "Rejected").
-   **Drag-and-Drop:** Move applications between status columns with a simple drag-and-drop interface.
-   **Add/Edit Applications:** A simple form to add new applications with key details:
    -   Company Name
    -   Job Title
    -   Job Description / URL
    -   Application Date
    -   Location (Remote/Hybrid/On-site)
    -   Salary (Optional)
-   **Detailed View:** Click on any application to view or edit all its details, including a section for personal notes, contacts, and interview schedules.

---

## Tech Stack

This project is built using the following technologies:

-   **Frontend:** React (with Vite), Tailwind CSS
-   **Backend & Database:** Firebase
    -   **Firestore:** NoSQL database for storing application data.
    -   **Firebase Authentication:** For handling user sign-up and login.
    -   **Firebase Hosting:** For production deployment.
-   **State Management:** React Context
-   **Tools:** Git, npm, Vite

---

## Installation Steps

To get a local copy up and running, follow these steps.

1.  **Clone the repository:**
    ```bash
    git clone [https://github.com/janedev/job-tracker-app.git](https://github.com/janedev/job-tracker-app.git)
    ```

2.  **Navigate to the project directory:**
    ```bash
    cd job-tracker-app
    ```

3.  **Install NPM dependencies:**
    ```bash
    npm install
    ```

4.  **Set up Firebase:**
    -   Go to the [Firebase Console](https://console.firebase.google.com/) and create a new project.
    -   In your project, add a new "Web" app.
    -   Copy the `firebaseConfig` object provided.
    -   Create a new file named `.env.local` in the root of your project.
    -   Add your Firebase config keys to this file (prefix with `VITE_` as this project uses Vite):
        ```env
        VITE_API_KEY=your_api_key
        VITE_AUTH_DOMAIN=your_auth_domain
        VITE_PROJECT_ID=your_project_id
        VITE_STORAGE_BUCKET=your_storage_bucket
        VITE_MESSAGING_SENDER_ID=your_messaging_sender_id
        VITE_APP_ID=your_app_id
        ```
    -   In the Firebase Console, go to "Authentication" and enable the "Email/Password" sign-in method.
    -   Go to "Firestore Database", create a new database, and set up your security rules.

5.  **Run the project:**
    ```bash
    npm run dev
    ```
    The application should now be running on `http://localhost:5173`.

---

## How to Use

1.  Navigate to the local URL (`http://localhost:5173`).
2.  Click "Sign Up" and create an account using your email and password.
3.  Once logged in, you will be directed to your main dashboard.
4.  Click the "Add New Application" button to open a form.
5.  Fill in the details for a job you've applied to and click "Save".
6.  Your new application will appear in the "Applied" column.
7.  You can drag and drop the application card to other columns (like "Interviewing" or "Offer") as your status changes.
8.  Click on any card to view its details, add notes, or make edits.

---

## Screenshots

![Login Page](./public/screenshots/login-page.png)
*Caption: User Login & Sign-up Page*

![Dashboard View](./public/screenshots/dashboard-view.png)
*Caption: Main dashboard view with applications sorted by status.*

![Add Application Modal](./public/screenshots/add-application-modal.png)
*Caption: Form for adding a new job application.*

---

## Contributors

-   **Jane Developer** - [https://github.com/janedev](https://github.com/janedev)

---

## License

This project is licensed under the **MIT License**. See the `LICENSE.md` file for details.
