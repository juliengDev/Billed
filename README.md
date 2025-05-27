# Billed - Expense Management SaaS

## Overview

Billed is a SaaS application designed for HR departments to manage and track employee expense reports. This project focuses on debugging and testing both the employee and admin user flows of the application, ensuring reliability through integration, unit, and manual end-to-end tests.

**🧪 Key Objectives:**
* Debug and fix frontend bugs using Chrome Debugger
* Write unit and integration tests using Jest
* Create a manual end-to-end test plan
* Deliver a functional product ready for production demo

---

## ✨ Features

* **Employee User Flow:**
    * Submit new expense reports via a form
    * Upload receipt images
    * View history of submitted bills
* **Admin User Flow:**
    * Review submitted expenses
    * Accept or reject expense reports
    * View attachments and employee details
* **Testing & Debugging:**
    * Unit and integration tests for employee interface
    * Debugging admin and employee interfaces using Chrome DevTools
    * Manual end-to-end test plan provided

---

## 🛠 Built With

* **JavaScript (ES6+)** - Core language
* **HTML / CSS / Bootstrap** - UI development
* **Jest** - Unit & integration testing
* **Testing Library (React & DOM)** - DOM interaction simulation
* **Chrome Debugger** - Runtime debugging
* **Node.js / Express** - Backend mock API
* **JSDOM / jsdom-environment** - Test environment for DOM manipulation

---

## ⚠️ Important Note

This application is **not deployed** and must be run locally. You will need to run both the frontend and backend to access the full features.

---

## 📦 Installation

1.  **Clone the repositories**

    ```bash
    # Frontend
    git clone [https://github.com/votre-utilisateur/Billed-frontend.git](https://github.com/votre-utilisateur/Billed-frontend.git)
    cd Billed-frontend

    # Backend (in a separate folder)
    git clone [https://github.com/OpenClassrooms-Student-Center/Billed-app-FR-Back.git](https://github.com/OpenClassrooms-Student-Center/Billed-app-FR-Back.git) ../Billed-backend
    ```

2.  **Install dependencies**

    **Frontend**

    ```bash
    npm install
    ```

    **Backend**

    ```bash
    cd ../Billed-backend
    npm install
    ```

3.  **Run the backend server**

    ```bash
    npm run run:dev
    ```

    The backend API will be available at `http://localhost:5678`.

4.  **Run the frontend app**

    ```bash
    cd ../Billed-frontend
    npm start
    ```

    The app will be accessible at `http://localhost:8080`.

---

## 🔐 Default Users

| Role     | Email             | Password   |
| :------- | :---------------- | :--------- |
| Employee | employee@test.tld | employee   |
| Admin    | admin@test.tld    | admin      |

---

## 🧪 Testing

Run all tests with coverage:

```bash
npm test
````

Generate HTML test report:

```bash
# After running tests, open the report manually
open coverage/lcov-report/index.html
```

Jest config is already set up with JSDOM and custom setup files.

-----

## 📄 Test Types Included

  * **Unit Tests:** Component-level logic (e.g., form validation, event handling)
  * **Integration Tests:** Full flows such as bill creation or user authentication
  * **Manual End-to-End Tests:** Documented separately (see `/tests/manual-tests.md`)

-----

## 📁 Project Structure

```
Billed-frontend/
├── __tests__/          # All Jest tests
├── src/
│   ├── app/            # App initialization
│   ├── containers/     # Page components (Bills, NewBill, Login, etc.)
│   ├── components/     # Shared UI components
│   ├── fixtures/       # Mock data
│   ├── assets/         # Styles, images, logos
│   └── router.js       # Routing logic
├── setup-jest.js       # Jest setup config
├── index.html          # App entry point
└── package.json
```

-----

## 🚧 Known Bugs Fixed

  * File input accepting invalid formats
  * Crash on form submission with missing fields
  * Bills page not rendering for certain users
  * Navigation sidebar inconsistencies

-----

## 📋 Manual Testing Plan

A complete manual test plan is available in the documentation:

  * Test all major employee and admin features
  * Validate edge cases (empty fields, incorrect formats, etc.)
  * Cross-browser testing using Chrome

-----

## 🤝 Contributing

Contributions are welcome\! Open issues or PRs for improvements or bugfixes.

1.  Fork the repository
2.  Create your feature branch (`git checkout -b feature/AmazingFeature`)
3.  Commit your changes (`git commit -m 'Add some AmazingFeature'`)
4.  Push to the branch (`git push origin feature/AmazingFeature`)
5.  Open a Pull Request

-----

## 👨‍💻 Author

  * 🌐 [Portfolio - Julien Gilbert](https://juliengilbert.com)
  * 🏆 [GitHub - @juliengDev](https://www.google.com/search?q=https://github.com/juliengDev)
  * 💼 [LinkedIn - Julien Gilbert](https://www.google.com/search?q=https://linkedin.com/in/juliengilbert)

-----

## 🎯 Acknowledgments

This project was completed as part of the Front-End Developer path at OpenClassrooms.
