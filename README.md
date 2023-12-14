# API for Registration and Login

Backend for API auth regsitration and login using nodejs and database mySQL

Endpoint
https://app-aqzbqeztja-et.a.run.app/

Register
URL
    /api/signup
Method
    POST
Request Body
    name as string
    email as string
    password as string
Response
    {
        "status": 201,
        "error": false,
        "message": "User Created",
        "user_id": 4
    }

Login
URL
    /api/login
Method
    POST
Request Body
    email as string
    password as string
Response
    {
    "status": 200,
    "error": false,
    "message": "Login successful",
    "access_token": "eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJpZCI6MywiaWF0IjoxNzAyNTYzMzYwLCJleHAiOjE3MDI1NjQ1NjB9.veBthI2tu94P3EytZtUhi-dDk6KhihCSNp3ZuZok598",
    "refresh_token": "eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJpZCI6MywiaWF0IjoxNzAyNTYzMzYwLCJleHAiOjE3MDI2NDk3NjB9.i-vnRmZX4QNzHUyXOePbvWfY6svSoAVv8uF5gXyD0wM"
}
