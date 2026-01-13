Flask REST API (GET & POST)

This repository contains a simple REST API built using Flask (Python).
The project demonstrates how to create GET and POST endpoints and test them using tools like Postman.

Features
Flask-based backend API
GET method to fetch user data
POST method to create user data
JSON request and response handling
Beginner-friendly project structure

--> Technologies Used
Python 3.x
Flask
Postman (for API testing)

--> Project Structure
Api.py
README.md

--> Installation & Setup
1) Clone the Repository
git clone https://github.com/muhammadsohaib17/Api_Making.git
cd Api_Making

2) Install Flask
pip install flask

3) Run the Server
python Api.py


You should see:
Running on http://127.0.0.1:5000/
--> API Endpoints

--> GET – Fetch User Data
GET /get-user/<user_id>
Example:
http://127.0.0.1:5000/get-user/1
Response:
{
  "user_id": "1",
  "name": "sohaib",
  "email": "sohaib.17@gmail.com"
}

Optional Query Parameter:
/get-user/1?extra=student

--? POST – Create User
POST /create-user
Request Body (JSON):
{
  "name": "Ali",
  "email": "ali@test.com"
}

Response:
{
  "name": "Ali",
  "email": "ali@test.com"
}

--> Testing the API
Use Postman or any REST client:
Set method to GET or POST
Set URL correctly

For POST requests:
Body → raw → JSON
Header:
Content-Type: application/json

--> Notes
This project is for learning and practice purposes
No database is used (data is static)
Suitable for beginners learning Flask APIs

--> Author
Muhammad Sohaib Khan

--> License
This project is open-source and free to use for learning.
