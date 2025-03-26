# Weak Website

[![License: MIT](https://img.shields.io/badge/License-MIT-blue.svg)](https://opensource.org/licenses/MIT)

A deliberately vulnerable web application designed for cybersecurity education and practice. This project demonstrates common web security vulnerabilities based on the OWASP Application Security Verification Standard (ASVS) Level 1 framework.

## 🚨 Security Warning

This application intentionally contains security vulnerabilities for educational purposes. **DO NOT** deploy this application in a production environment or on a public-facing server. It should only be run in controlled, isolated environments for learning and training.

## 🌟 Features

- Interactive vulnerable components showcasing OWASP ASVS Level 1 vulnerabilities
- Full-stack architecture with separate client and server applications
- Modern tech stack using React, TypeScript, NestJS, and MySQL
- Docker setup for easy deployment and isolation
- Educational annotations throughout the codebase

## 🏗️ Architecture

- **Client**: React application with TypeScript and ShadCN UI components
- **Server**: NestJS backend with TypeScript and TypeORM for database operations
- **Database**: MySQL database with pre-configured vulnerable data models

## 🚀 Getting Started

### Prerequisites

- [Docker](https://www.docker.com/get-started) and Docker Compose
- [Node.js](https://nodejs.org/) (v18 or higher) for local development

### Development Setup

1. Start the development environment:
   ```bash
   docker-compose -f docker-compose.dev.yml up --build -d
   ```

2. Access the application:
   - Client: http://localhost:8081
   - Server: http://localhost:3000
   - API Documentation: http://localhost:3000/api

### Production Setup

1. Build and start the production containers:
   ```bash
   docker-compose up --build -d
   ```

## 💻 Local Development

### Client

```bash
cd client
npm install
npm run dev
```

### Server

```bash
cd server
npm install
npm run start:dev
```

## 📚 Vulnerabilities Implemented

This project implements vulnerabilities based on the OWASP ASVS Level 1 requirements, including:

- Authentication weaknesses (V2)
- Session management flaws (V3)
- Access control issues (V4)
- Input validation failures (V5)
- Cryptographic problems (V6)
- Error handling and logging issues (V7)
- Data protection weaknesses (V8)
- Communications security flaws (V9)
- Malicious code issues (V10)
- Business logic vulnerabilities (V11)
- File and resource vulnerabilities (V12)
- API and web service issues (V13)
- Configuration problems (V14)

## 🛠️ Technology Stack

- **Frontend**: React, TypeScript, ShadCN UI, TailwindCSS, Vite
- **Backend**: NestJS, TypeScript, TypeORM
- **Database**: MySQL
- **Containerization**: Docker, Docker Compose

## 📜 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## ⚠️ Disclaimer

This application is designed for educational and training purposes only. The maintainers are not responsible for any misuse of the vulnerabilities demonstrated in this project.