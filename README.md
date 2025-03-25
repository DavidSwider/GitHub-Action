# GitHub-Action

# Full-Stack Application with Cypress Testing & GitHub Actions

## Table of Contents
- [Description](#description)
- [Features](#features)
- [Technologies Used](#technologies-used)
- [Installation](#installation)
- [Development Workflow](#development-workflow)
- [Testing with Cypress](#testing-with-cypress)
- [Deployment](#deployment)
- [Contributing](#contributing)
- [Contact](#contact)

---

## Description
This project is a **full-stack application** that incorporates **Cypress component testing** and **automated deployment** using **GitHub Actions and Render**. The application follows a structured development workflow where new features are tested before merging to the main branch.

---

## Features

### 🛠 Development Workflow with GitHub Actions
- Developers must create **Pull Requests (PRs) to the `develop` branch** before merging to `main`.
- Upon creating a PR, **GitHub Actions triggers Cypress tests** to ensure feature stability.
- Once **all tests pass**, developers can merge changes into `develop`.
- **Merging `develop` into `main`** triggers another GitHub Action to **automatically deploy** the application to **Render**.

### ✅ Automated Testing with Cypress
- **Component tests run on every PR** using GitHub Actions.
- Developers can review test results directly on **GitHub** before merging.
- Ensures that each feature is functional before deployment.

### 🚀 Continuous Deployment on Render
- Code pushed to the `main` branch **automatically deploys to Render**.
- Ensures a streamlined **CI/CD pipeline** for quick and efficient updates.

---

## Technologies Used
- **Frontend:** React.js
- **Backend:** Node.js & Express.js
- **Database:** MongoDB
- **Testing:** Cypress
- **CI/CD:** GitHub Actions
- **Hosting:** Render
- **Version Control:** Git & GitHub

---

## Installation
To run the project locally, follow these steps:

1. **Clone the Repository:**
   ```sh
   git clone https://github.com/DavidSwider/GitHub-Action.git
   cd GitHub-Action
   ```  
2. **Install Dependencies:**
   ```sh
   npm install
   ```  
3. **Start the Backend Server:**
   ```sh
   npm run build
   ```  
4. **Seed the App:**
   ```sh
   npm run seed
   ```  
5. **Start the Frontend:**
   ```sh
   npm run start
   ```  
6. Open `http://localhost:3000/` in your browser.

---

## Development Workflow

1. Create a **new feature branch** from `develop`:
   ```sh
   git checkout -b feature-branch-name develop
   ```
2. Develop your feature and commit changes.
3. Push the feature branch to GitHub:
   ```sh
   git push origin feature-branch-name
   ```
4. Create a **Pull Request (PR) to `develop`**.
5. **GitHub Actions will run Cypress tests automatically**.
6. Once tests pass, merge into `develop`.
7. When ready, merge `develop` into `main`.
8. **GitHub Actions will trigger automatic deployment to Render**.

---

## Testing with Cypress

npx cypress run --browser electron:
```sh
npm run test
```
npx cypress run --component:
```sh
npm run test-component
```
npx cypress open:
```sh
npm run test-gui
```
All PRs to `develop` will **automatically run Cypress tests** via **GitHub Actions**.

---

## Deployment
- The application is automatically deployed to **Render** when code is pushed to the `main` branch.
- Deployment logs can be checked on Render's dashboard.
🔗 Render: [Deployment](https://github-action-bsv7.onrender.com) 
---

## Contributing
We welcome contributions! Follow these steps:
1. Fork the repository.
2. Create a feature branch from `develop`.
3. Commit and push your changes.
4. Open a Pull Request (PR) to `develop`.

---

## Contact
📧 Email: Davidswider6@gmail.com  
🔗 GitHub: [YourGitHubProfile](https://github.com/DavidSwider/GitHub-Action)    
🔗 GitHubGist: [YourGitHubGist](https://github.com/DavidSwider/GitHub-Action)  
---

This **README** provides a structured overview of the project.🚀

