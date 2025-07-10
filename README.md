# Advertisement System – Unfinished School Project

## Description

This is an unfinished assessment project developed during the 4th year of vocational high school as part of an _Advanced Web Application Programming_ course. The backend is fully functional, but the frontend is in an early development stage and lacks many pages and features.

During the presentation, I used [Render](https://render.com/) to deploy a Dockerized version of the backend. Because of this, both the frontend and backend have specific preferences depending on whether the project is run locally or deployed on an external server.

In the case of the frontend:
- `npm start` starts the React app locally and connects to a locally running Spring Boot backend.
- `npm run deploy` starts the React app locally but connects to the backend deployed on Render.

The backend was developed using IntelliJ IDEA Community Edition. To run it, a custom Run/Debug configuration is required. This configuration uses the standard Maven template with the command: _spring-boot:run_ and the environment variable: _spring.profiles.active=local_ adjusted according to the environment.

In [this directory](backend/SystemOgloszeniowy/src/main/resources), you'll find two separate configuration files corresponding to the different deployment environments.

Although the project is unfinished, it was still awarded the highest possible grade.

## Used Frameworks

### Backend
- Spring Boot
- Java 17
- Liquibase
- PostgreSQL 14
- Docker (optional, for deployment)

### Frontend
- React.js + Webpack
- Bootstrap
- React Toastify
	
## 📄 Project requirements

[Project requirements (in Polish)](https://drive.google.com/file/d/1B1EeGr7Roi5OVLkDcZi8VIX_oyW9Z71x/view?usp=sharing)