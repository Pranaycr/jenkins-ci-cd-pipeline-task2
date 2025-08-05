# Jenkins CI/CD Pipeline — Task 2

## Submitted by:
Chinnaramaiahgari Pranay Goud

---

## Objective:
Automate the process of building, testing, and deploying a Node.js application using Jenkins Pipeline as part of a CI/CD workflow.

---

## Tools & Technologies Used:
- Jenkins
- Docker
- Git & GitHub
- Visual Studio Code (VS Code)
- Node.js

---

## Pipeline Stages:
1. **Build** — Install dependencies and build the application.
2. **Test** — Run test cases (dummy echo for now).
3. **Deploy** — Deploy application (e.g., Docker image push).

---

## Jenkinsfile:
The Jenkins pipeline is defined in the **Jenkinsfile** using Declarative Pipeline Syntax.
```groovy
pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                echo 'Building the project...'
            }
        }
        stage('Test') {
            steps {
                echo 'Running tests...'
            }
        }
        stage('Deploy') {
            steps {
                echo 'Deploying the application...'
            }
        }
    }
}
