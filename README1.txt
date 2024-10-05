# Customer Accounts Microservice - DevOps Capstone Project

## Overview
This capstone project demonstrates the end-to-end creation of a RESTful Customer Accounts microservice using agile methodologies, Test-Driven Development (TDD), and modern DevOps practices.

## Key Features
- **Agile Planning:** Created a GitHub repository and Kanban board with user stories and sprint plans.
- **Microservice Development:** Developed RESTful API with Flask using TDD, achieving over 95% code coverage.
- **CI/CD Pipeline:** Configured GitHub Actions to automate build, linting, testing, and code coverage.
- **Security Enhancements:** Implemented Flask-Talisman and Flask-CORS for secure headers and CORS policies.
- **Containerization & Deployment:** Built Docker images, deployed to Kubernetes/OpenShift with automated pipelines using Tekton.
- **Database Integration:** Configured PostgreSQL for persistent data storage in Kubernetes.

## Tools & Technologies
- **Languages & Frameworks:** Python, Flask
- **Version Control:** Git, GitHub
- **CI/CD Tools:** GitHub Actions, Tekton
- **Containerization:** Docker, Kubernetes, OpenShift
- **Security:** Flask-Talisman, Flask-CORS
- **Database:** PostgreSQL
- **Testing Tools:** Nose, Flake8

## Development Process
1. **Agile Sprint Planning:**
   - Created a backlog with user stories.
   - Managed sprints and tracked progress using GitHub Kanban.
  
2. **Test-Driven Development (TDD):**
   - Developed functions for CRUD operations (create, read, update, delete) and wrote test cases.
   - Ran `nosetests` to ensure passing unit tests and achieved 95% code coverage.

3. **Continuous Integration (CI):**
   - Configured a GitHub Actions workflow triggered by pull requests or pushes.
   - Linted the code using Flake8 and ran tests with coverage analysis.

4. **Security Enhancements:**
   - Added security headers and CORS policies using Flask-Talisman and Flask-CORS.
   - Applied TDD to implement and test security features.

5. **Containerization & Deployment:**
   - Created a Dockerfile for the microservice, built, and deployed the image to Kubernetes/OpenShift.
   - Deployed PostgreSQL as the service's database in Kubernetes.

6. **Automated Deployment:**
   - Built a Tekton pipeline to automate the CI/CD process, including building, testing, and deploying the service to Kubernetes.

## Running the Project Locally
1. **Clone the Repository:**
   ```bash
   git clone https://github.com/elisamni/devops-capstone-project.git
   cd devops-capstone-project
