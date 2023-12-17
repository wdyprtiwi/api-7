
# API for Phisheye Application

Backend for API auth regsitration, login, report link using express, nodejs, and database MySQL 

Endpoint
--
https://app-aqzbqeztja-et.a.run.app/
Update: https://app-5hl7lkua7q-uc.a.run.app

Register
--

### URL <br>
    /api/signup

### Method
    POST
    
### Request Body
   - name as string <br>
   - email as string <br>
   - password as string <br>

### Response
    {
        "status": 201,
        "error": false, 
        "message": "User Created",
        "user_id": 4
    }

Login
--

### URL
    /api/login

### Method
    POST

### Request Body
- email as string <br>
- password as string <br>

### Response
    {
        "status": 200,
        "error": false,
        "message": "Login successful",
        "access_token": "eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJpZCI6MywiaWF0IjoxNzAyNTYzMzYwLCJleHAiOjE3MDI1NjQ1NjB9.veBthI2tu94P3EytZtUhi-dDk6KhihCSNp3ZuZok598",
        "refresh_token": "eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJpZCI6MywiaWF0IjoxNzAyNTYzMzYwLCJleHAiOjE3MDI2NDk3NjB9.i-vnRmZX4QNzHUyXOePbvWfY6svSoAVv8uF5gXyD0wM"
    }

Report Link
--

### URL
    /api/report-link

### Method
    POST

### Request Body
- link as string

### Response
    {
    "status": 201,
    "error": false,
    "message": "Report link successful",
    "link_id": 1
    }
