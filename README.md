# JS-Core-4.3.9
1. Регистрируемся (Registration) POST: https://blog.kata.academy/api/user
{
  "user": {
    "username": "vvnezapnopwnz",
    "email": "vvnezapnopwnz@gmail.com",
    "password": "vvnezapnopwnz"
  }
}

2. Логинимся (Authentication) POST: https://blog.kata.academy/api//users/login
Login for existing user
{
  "user": {
    "email": "vvnezapnopwnz@gmail.com",
    "password": "vvnezapnopwnz"
  }
}
Response: {
    "user": {
        "username": "vvnezapnopwnz",
        "email": "vvnezapnopwnz@gmail.com",
        "token": "eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJpZCI6IjYzMjVjM2UxM2NmNzA1MWIwMDgyYTQ2NCIsInVzZXJuYW1lIjoidnZuZXphcG5vcHdueiIsImV4cCI6MTY2OTA0NTcxOCwiaWF0IjoxNjYzODYxNzE4fQ.XwGyQQo6a7YC5fd1-7lhAfxUvFCAFL1VqiGaameU0ro"
    }
}
3. Используя заголовок авторизации получить данные текущего пользователя (Endpoints -> Get Current User) GET: https://blog.kata.academy/api/user
Gets the currently logged-in user
Auth
  Token: eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJpZCI6IjYzMjVjM2UxM2NmNzA1MWIwMDgyYTQ2NCIsInVzZXJuYW1lIjoidnZuZXphcG5vcHdueiIsImV4cCI6MTY2OTA0NTE4MiwiaWF0IjoxNjYzODYxMTgyfQ.RZmf9ryubkkSy-WAOfWPSVq2xQbpssnMN9K6Yhu1Fe4
