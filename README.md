# Lab 1: Node.js and Express Server
live deployment url: https://backend-development-lab-1.onrender.com/

**Subject:** Backend Development Fundamentals  
**Year/Term:** Year II, Term II  
**University:** Aurora Deemed to be University  
**Faculty:** Mr. Joel Prashanth D

## 1. Student Details

| Field | Details |
|---|---|
| Name | Tarendra Reddy |
| Registration Number | 252U1R9157 |
| Section | S-26 |

## 2. Project Objective

The objective of this lab is to understand the fundamentals of creating and running a backend server using Node.js and Express.js. It covers project initialization using npm, installing dependencies, creating an HTTP server, handling routes, returning JSON responses, generating the current date and time, using HTTP status codes, and handling unknown routes.

The project includes a basic Node.js HTTP server and an Express server that listens on port 3000.

## 3. Technologies Used

- Node.js
- Express.js
- npm
- JavaScript (CommonJS)
- HTTP and JSON response handling
- Visual Studio Code

## 4. Project Folder Structure

```text
lab-01/
├── plain-server.js
├── server.js
├── package.json
├── package-lock.json
├── README.md
├── .gitignore
└── screenshots/
    ├── home.png
    ├── about.png
    ├── time.png
    └── 404.png
```

## 5. Installation and Execution

### Prerequisites

- Node.js and npm installed on the computer.
- Visual Studio Code or Antigravity editor.

### Install Dependencies

Open the terminal in the project directory and run:

```bash
npm install
```

If Express is not installed, run:

```bash
npm install express
```

### Run the Plain Node.js Server

Execute the following command:

```bash
node plain-server.js
```

The server listens on port 3000. Open the following URL in your browser:

`http://localhost:3000`

**Expected response:**

```text
Hello
```

Stop the server by pressing `Ctrl + C`.

### Run the Express Server

Execute the following command:

```bash
node server.js
```

Open the following URL in your browser:

`http://localhost:3000`

Keep the terminal running while testing the routes. Press `Ctrl + C` to stop the server.

**Note:** Only one server should run on port 3000 at a time.

## 6. Endpoints

| HTTP Method | Path | Description | Expected Status Code |
|---|---|---|---|
| GET | `/` | Returns a welcome message | 200 OK |
| GET | `/about` | Returns student information in JSON format | 200 OK |
| GET | `/time` | Returns the current date and time using `new Date()` | 200 OK |
| GET | Any unknown path | Returns a page-not-found message | 404 Not Found |

### Example Requests

- Home: `http://localhost:3000/`
- About: `http://localhost:3000/about`
- Time: `http://localhost:3000/time`
- Unknown route: `http://localhost:3000/unknown`

## 7. Screenshots

Save screenshots of the working routes in the `screenshots/` folder.

### Home Route

![Screenshot](./Screenshot%202026-10-27%20103913.png)

### About Route

![Screenshot](./Screenshot%202026-10-27%20103948.png)

### Time Route

![Screenshot](./Screenshot&202026-10-27%20104012.png)

### 404 Route

![Screenshot](./Screenshot%202026-10-27%20104039.png)

## 8. Deployment

The application can be deployed using a Node.js-compatible hosting service such as Render or Railway. Configure the hosting service to install dependencies using `npm install` and start the application using `node server.js`.

For deployment, the server should use the port provided by the hosting environment when available.

**Provided deployment URL:**  
https://backend-development-lab-1.onrender.com/

Verify that the deployed application is working before submitting the live URL. If deployment is unsuccessful, explain the reason in this README and include screenshots of the endpoints tested locally or through Postman.

## 9. Problems Faced and Solutions

| Problem | Solution |
|---|---|
| Understanding npm project setup | Used `npm init -y` to create `package.json`. |
| Express was not available initially | Installed Express using `npm install express`. |
| Different routes needed different response formats | Used `res.send()` for text and `res.json()` for JSON. |
| Generating the current date and time | Used `new Date()` in the `/time` route. |
| Handling unknown URLs | Added middleware to return a 404 response. |
| PowerShell blocked the npm command | Used `npm.cmd` to execute npm commands when required. |

## 10. Learning Outcomes

- Learned how to initialize a Node.js project using npm.
- Understood the purpose of `package.json`, `package-lock.json`, and `node_modules`.
- Installed and used Express.js.
- Created an Express server listening on port 3000.
- Implemented GET routes and returned text and JSON responses.
- Generated the current date and time using `new Date()`.
- Used HTTP status codes 200 and 404.
- Learned how to document and prepare a backend project for GitHub submission.

## 11. Git Hygiene

Create a `.gitignore` file in the project root with the following entries:

```text
node_modules/
.env
```

Do not commit `node_modules`, `.env` files, passwords, API keys, or other secret information to GitHub.

## 12. GitHub Repository

**Repository URL:**  
https://github.com/tarendra-reddy/Backend-Development-Lab-1.git

The repository contains the source code and documentation for Lab 1: Node.js and Express Server.

