# Customer Accounts Microservice - DevOps Capstone Project

![Build Status](https://github.com/elisamni/devops-capstone-project/actions/workflows/ci-build.yaml/badge.svg)
 
[![License](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](https://opensource.org/licenses/Apache-2.0)
[![Python 3.9](https://img.shields.io/badge/Python-3.9-green.svg)](https://shields.io/)

This repository contains the starter code for the project in [**IBM-CD0285EN-SkillsNetwork DevOps Capstone Project**](https://www.coursera.org/learn/devops-capstone-project?specialization=devops-and-software-engineering) which is part of the [**IBM DevOps and Software Engineering Professional Certificate**](https://www.coursera.org/professional-certificates/devops-and-software-engineering)

## Overview
This capstone project demonstrates the end-to-end creation of a RESTful Customer Accounts microservice using agile methodologies, Test-Driven Development (TDD), and modern DevOps practices.

## Project layout

The code for the microservice is contained in the `service` package. All of the test are in the `tests` folder. The code follows the **Model-View-Controller** pattern with all of the database code and business logic in the model (`models.py`), and all of the RESTful routing on the controller (`routes.py`).

```text
├── service         <- microservice package
│   ├── common/     <- common log and error handlers
│   ├── config.py   <- Flask configuration object
│   ├── models.py   <- code for the persistent model
│   └── routes.py   <- code for the REST API routes
├── setup.cfg       <- tools setup config
└── tests                       <- folder for all of the tests
    ├── factories.py            <- test factories
    ├── test_cli_commands.py    <- CLI tests
    ├── test_models.py          <- model unit tests
    └── test_routes.py          <- route unit tests
```

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
**Clone the Repository:**
   ```bash
git clone https://github.com/elisamni/devops-capstone-project.git
cd devops-capstone-project
```

## Build and Run with Docker:
```bash
docker-compose up --build
```
## Conclusion

This capstone project highlights the application of DevOps practices to build a secure, scalable, and automated microservice. The project involved the integration of CI/CD pipelines, containerization, Kubernetes deployment, and security enhancements, all developed and tested with TDD.

## Author

[John Rofrano](https://www.coursera.org/instructor/johnrofrano), Senior Technical Staff Member, DevOps Champion, @ IBM Research, and Instructor @ Coursera

## License

Licensed under the Apache License. See [LICENSE](LICENSE)
