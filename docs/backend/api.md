# API Overview

The backend exposes a RESTful API for managing users and tasks.  
All endpoints respond in JSON format and follow consistent validation and error patterns.

## Base URL

http://localhost:5000/swagger


## Authentication

Authentication is handled using JWT tokens.

### Login

**POST** `/auth/login`

#### Request

```json
{
  "email": "user@example.com",
  "password": "string"
}
```
#### Response

```json
{
  "token": "jwt-token-string",
  "expiresIn": 3600
}
```

### Register

#### Body

```json
{
  "email": "user@example.com",
  "password": "string"
}
```

## Task Endpoints

### Get All Tasks

**GET** `/tasks`


