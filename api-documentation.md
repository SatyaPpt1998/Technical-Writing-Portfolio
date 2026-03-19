# Login API Documentation

## Endpoint
POST /api/login

## Request Body
{
  "username": "user123",
  "password": "password123"
}

## Response
200 OK
{
  "message": "Login successful",
  "token": "abc123xyz"
}

## Error Response
401 Unauthorized
{
  "error": "Invalid credentials"
}
