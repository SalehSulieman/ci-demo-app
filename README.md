# CI/CD Fundamentals Lab — CI Demo App

A foundational DevOps project demonstrating **Continuous Integration** using GitHub Actions on a container-ready Node.js application.

---

## Overview
This lab introduces CI/CD pipeline automation.  
Each code push triggers automated build and test workflows to ensure repository integrity before deployment.  
The project uses a lightweight Node.js server as the build target, validating that the pipeline executes correctly on every commit.

---

## Workflow Summary
| Step | Description |
|------|--------------|
| **Trigger** | Runs automatically on every push or pull request to the `main` branch. |
| **Checkout** | Retrieves repository source code. |
| **Setup Node.js** | Initializes Node.js 18 on the runner. |
| **Install Dependencies** | Executes `npm ci` for a clean dependency install. |
| **Run Tests** | Executes placeholder tests to validate configuration. |
| **Build Step** | Starts the Node.js app build to confirm successful run. |

---

## Repository Structure
ci-demo-app/
├── src/
│ └── server.js # Minimal HTTP server
├── .github/
│ └── workflows/
│ └── ci.yml # CI pipeline definition
├── package.json # Node.js metadata and scripts
└── README.md # Documentation


---

## Local Usage
```bash
git clone https://github.com/SalehSulieman/ci-demo-app.git
cd ci-demo-app
npm install
npm start
```
Then visit http://127.0.0.1:3000 to verify output.

##Technologies Used

Node.js 18

GitHub Actions (YAML workflows)

Ubuntu-based CI runners

##Why This Matters

This lab establishes your foundation in Continuous Integration, ensuring that codebases remain buildable and testable across all commits — a core DevOps principle preceding containerization and automated deployment.

##Author

Saleh Sulieman — Computer Engineering Student @ Ostim Teknik University
