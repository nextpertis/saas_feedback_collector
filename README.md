# SaaS Feedback Collector

This repository contains a full-stack application for collecting SaaS feedback, consisting of a Spring Boot backend and an Angular frontend.

## Table of Contents

- [SaaS Feedback Collector](#saas-feedback-collector)
  - [Table of Contents](#table-of-contents)
  - [Overview](#overview)
  - [Backend](#backend)
    - [Technologies Used](#technologies-used)
    - [Getting Started (Backend)](#getting-started-backend)
  - [Frontend](#frontend)
    - [Technologies Used](#technologies-used-1)
    - [Getting Started (Frontend)](#getting-started-frontend)

## Overview

The SaaS Feedback Collector is a web application designed to gather feedback from users of SaaS products. It is built as a monolithic application with a Java Spring Boot backend providing the API and business logic, and an Angular frontend providing the user interface.

## Backend

### Technologies Used

- **Spring Boot:** A framework for building production-ready Spring applications.
- **Java 17:** The primary programming language.
- **Maven:** The build automation tool.
- **AWS SDKs:** Integration with various AWS services (Secrets Manager, Pinpoint, DynamoDB, S3, SQS).
- **AWS SAM (Serverless Application Model):** For defining and deploying serverless resources (though not explicitly found in this directory, it's inferred from similar projects).
- **Stripe:** For payment processing (inferred from `pom.xml`).
- **Swagger UI:** For API documentation.

### Getting Started (Backend)

1. **Build the project:**
   ```bash
   cd backend
   mvn clean package
   ```
2. **Run locally:**
   ```bash
   java -jar target/saasfeedbackcollector-0.0.1-SNAPSHOT.jar
   ```
   (Note: If deployed as a Lambda, local execution might require SAM CLI.)

## Frontend

### Technologies Used

- **Angular:** A platform for building mobile and desktop web applications.
- **TypeScript:** The primary programming language for Angular.
- **npm/Yarn:** For package management.

### Getting Started (Frontend)

1. **Install dependencies:**
   ```bash
   cd frontend
   npm install # or yarn install
   ```
2. **Run locally:**
   ```bash
   ng serve
   ```
   This will start a development server, typically accessible at `http://localhost:4200/`.
3. **Build for production:**
   ```bash
   ng build --configuration production
   ```
   The build artifacts will be stored in the `dist/` directory.