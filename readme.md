# FastAPI User Authentication with OAuth2 and JWT

This project demonstrates how to implement user authentication and authorization in a FastAPI application using OAuth2 with JWT (JSON Web Tokens).

## Overview

This FastAPI application provides endpoints for user authentication, token generation, and access control for protected resources. It utilizes OAuth2 with JWT tokens for secure authentication and authorization.

## Features

- **User Authentication**: Users can authenticate using their username and password.
- **JWT Token Generation**: Upon successful authentication, JWT tokens are generated.
- **Token-Based Authorization**: Endpoints are protected using token-based authorization.
- **User Profile**: Users can access their own profile information.
- **Protected Resources**: Certain resources are accessible only to authenticated users with valid tokens.

## Installation

1. Clone the repository to your local machine.
2. Install dependencies using `pip install -r requirements.txt`.
3. Run the FastAPI server using `uvicorn main:app --reload`.

## Usage

- **Authentication**: Send a POST request to `/token` with valid credentials to obtain a JWT token.
- **Access Protected Routes**: Use the generated JWT token to access protected routes.
- **User Profile**: Access `/users/me/` to retrieve the current user's profile information.

## Endpoints

- **POST /token**: Generate JWT token by authenticating with username and password.
- **GET /users/me/**: Retrieve the current user's profile information.
- **GET /users/me/items**: Retrieve items owned by the current user.

## Dependencies

- **FastAPI**: A modern web framework for building APIs with Python.
- **Pydantic**: Data validation and settings management using Python type annotations.
- **Passlib**: Password hashing library for secure password storage and verification.
- **PyJWT**: JSON Web Token implementation for Python.
- **Uvicorn**: ASGI server implementation used to run the FastAPI application.

## Contributing

Contributions are welcome! Feel free to submit pull requests or open issues for any improvements or bug fixes.
