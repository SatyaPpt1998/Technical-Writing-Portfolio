# Login API Documentation

## Overview
This API allows users to authenticate and receive an access token.

## Base URL
https://api.example.com

## Endpoint
POST /api/login

## Headers
Content-Type: application/json

## Request Body
{
  "username": "string",
  "password": "string"
}

## Sample Request
POST /api/login
{
  "username": "user123",
  "password": "password123"
}

## Success Response
200 OK
{
  "message": "Login successful",
  "token": "abc123xyz"
}

## Error Responses

### 400 Bad Request
{
  "error": "Missing fields"
}

### 401 Unauthorized
{
  "error": "Invalid credentials"
}

## Notes
- Ensure all fields are provided
- Token must be used for authenticated APIs
