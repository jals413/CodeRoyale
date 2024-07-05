# CodeRoyale

CodeRoyale is an online judge platform where users can login, access a list of problems, solve them, and receive verdicts on their solutions. The platform is built with Next.js, ensuring a modern and efficient user experience.

## Table of Contents
1. [Description](#description)
2. [Features](#features)
3. [How to Use](#how-to-use)
4. [Technologies Used](#technologies-used)
5. [Setup Locally](#setup-locally)
6. [Architecture Overview](#architecture-overview)
7. [Database and ER Diagram](#database-and-er-diagram)
8. [How to Contribute](#how-to-contribute)
9. [Links](#links)
10. [Contributors](#contributors)
11. [License](#license)

## Description

CodeRoyale is a web application designed to provide a seamless experience for users to solve programming problems and receive automated verdicts. It leverages a microservice architecture for scalability and robustness.

## Features

- **Online Judge**: Users can login and solve programming problems, receiving automated verdicts.
- **Microservice Architecture**:
  - **User Management Server**: Built with Node.js, handles CRUD operations on users.
  - **Code Execution Server**: Built with Go, executes code in a sandbox environment and provides verdicts.
- **Scalability**: Capable of handling up to 1000 concurrent users.
- **Upcoming Features**: Contest feature will be available soon.
- **Next.js**: A React framework for building fast and user-friendly static and dynamic web applications.
- **TypeScript**: Ensures robust and error-free code.
- **Tailwind CSS**: Provides utility-first CSS for rapid UI development.
- **Vercel**: Deployment platform for modern web projects.

## How to Use

To start the development server, run:

```bash
npm run dev
```

Open [http://localhost:3000](http://localhost:3000) in your browser to see the application.

## Technologies Used

- **Next.js**
- **Node.js**
- **Go**
- **TypeScript**
- **Tailwind CSS**
- **Vercel**
- **MongoDB**

## Setup Locally

To set up the project locally, follow these steps:

1. Clone the repository: 
   ```bash
   git clone https://github.com/Low4ey/CodeRoyale.git
   ```
2. Navigate to the project directory: 
   ```bash
   cd CodeRoyale
   ```
3. Install dependencies:
   ```bash
   npm install
   ```
4. Start the development server:
   ```bash
   npm run dev
   ```

## Architecture Overview

### Architecture Diagram
![Architecture Diagram](https://github.com/jals413/CodeRoyale/assets/63969102/0562329d-7985-44c0-9fc0-fbec96ad73fb)

### Components

1. **Frontend (Next.js)**
   - User Interface
   - Problem Listings
   - Submission Forms
   - User Authentication

2. **Backend**
   - **User Management Service (Node.js)**
     - Handles CRUD operations for users
   - **Code Execution Service (Go)**
     - Executes user code in a sandbox environment
     - Returns verdicts based on execution results
   - **Database (MongoDB)**
     - Stores user data, problems, submissions, test cases, etc.

3. **APIs**
   - RESTful APIs for communication between services

## Database and ER Diagram

### ER Diagram
![ER Diagram](path/to/your/ER-diagram.png)

The database consists of several interconnected schemas:

- **User Schema**: Manages user information and authentication.
- **Problem Schema**: Stores problems with details like title, content, tags, and difficulty.
- **Submission Schema**: Tracks user submissions, including code and status.
- **TestCase Schema**: Contains test cases for each problem.
- **ProblemSetter Schema**: Manages problem setters' details and approvals.
- **Editorial Schema**: Stores editorial content for problems.

## How to Contribute

We welcome contributions! To contribute:

1. **Fork the Repository**: Create a fork of this repository.
2. **Create a Branch**: Create a new branch for your feature or bug fix.
3. **Make Changes**: Implement your changes in the new branch.
4. **Create a Pull Request**: Submit a pull request with a detailed description of your changes.

### Issues

If you encounter any issues or have suggestions, please create an issue on the [Issues](https://github.com/Low4ey/CodeRoyale/issues) page.

### Pull Requests

We encourage you to submit pull requests for any improvements or fixes. Make sure to follow the project's coding guidelines and provide detailed descriptions of your changes.

## Links

- [Repository](https://github.com/Low4ey/CodeRoyale)
- [Issues](https://github.com/Low4ey/CodeRoyale/issues)

## Contributors

- [Low4ey](https://github.com/Low4ey)
- [jals413](https://github.com/jals413)
  
## License

This project is open-source and available under the [MIT License](LICENSE).
