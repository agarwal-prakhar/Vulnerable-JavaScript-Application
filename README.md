<div align="center">
<h1>
  Vulnerable JavaScript Application
</h1>
  
[![License](https://img.shields.io/badge/license--_red.svg)](https://opensource.org/licenses)
[![contributions welcome](https://img.shields.io/badge/contributions-welcome-brightgreen.svg?style=flat)](https://github.com/github.com/payatu/vuln-nodejs-app/issues) 
[![version](https://img.shields.io/badge/version-v1.0-blue.svg?style=flat)](https://github.com/payatu/vuln-nodejs-app)
<br><br>
</div>

Vulnerable JavaScript application is developed for web application penetration testers, developers and secure code review. It can be easily deployed using docker or by manual install complete steps are provided below. this application will help you in learning how to find vulnerabilities in web applicaiton using black box, white box approach and in learning how to fix them.
  
<h2> How to use it?</h2>
  
  - Black box testing: Deploy the appplication using docker and start solving the exercises.
  - Secure code review:  Manually install the application this will allow you to use debugger while solving the exercises and will help you in finding vulnerabilities in application code.
  - Developers: Identify vulnerabilities in application code & try to fix them.

<h2>Tech Stack</h2>

- NodeJS
- Application design pattern: MVC
- Web framework: Express
- Template Engine: EJS
- SQL Database: MySQL
- NoSQL Database: MongoDB
- React to cover ReactJS exercise
- JWT for authentication
- GraphQL
- Socket.IO
- Docker


<br>
</a>

<h2> Complete list of exercises </h2>

1. Command Injection
2. Insecure Deserialization
3. SQL Injection
4. XML external entity injection
5. XSS
6. Server Side Template Injection
7. JWT weak secret
8. Insecure direct object references
9. SSRF via PDF generator
10. postMessage XSS
11. postMessage CSRF
12. CORS Information Disclosure
13. CORS CSRF
14. 2FA Insecure Implementation
15. Cross-Site WebSocket Hijacking
16. ReactJS href XSS
17. GraphQL SQL Injection
18. GraphQL CSRF
19. GraphQL IDOR
20. XSS using SVG file uplaod


<h2> Installation </h2>

<h3> Using docker-compose </h3> 

1. Clone the repository.

```bash
git clone https://github.com/agarwal-prakhar/Vulnerable-JavaScript-Application.git
cd ./Vulnerable-JavaScript-Application
```
2. Download and build the image.

```bash
docker-compose up --build -d
```

3. Start the application.
```
docker-compose up -d  # Remove -d flag if you want to see logs
```
access the application http://localhost:9000

### Manual install

1. Clone the repository.

```bash
git clone [https://github.com/agarwal-prakhar/Vulnerable-JavaScript-Application.git]
cd ./Vulnerable-JavaScript-Application
```

2. Create **MySQL** database.

```bash
$ mysql -u <mysql_user> -p

mysql> create database vuln_js_app;

```

3. Update your MySQL and MongoDB database username and password inside **.env** file.

```html
DB_PORT=3306
DB_NAME=vuln_js_app
DB_USER=vuln_js_user
DB_PASS=passw0rd
HOST_PORT=9000
JWT_SECRET=secret
MONGODB_SERVER=localhost
MONGODB_ADMINUSERNAME=
MONGODB_ADMINPASSWORD=
```


4. Install dependencies.

```bash
npm install
```

5. Build React frontend.

```bash
npm run build
```

6. Start the server

```bash
node server.js
```
You can now access the application at http://localhost:9000
<br>






