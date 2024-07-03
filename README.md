## Introduction

This project showcases how to integrate Spring Security into a Spring Boot application. It includes examples of authentication, authorization, and various security configurations.

## Features

- User Authentication
- Role-Based Authorization
- JWT Token Security
- Custom Login and Registration
- In-Memory and H2 Database Authentication
- Method-Level Security

### Default Credentials

- **Username**: `user`
- **Password**: `password` (or check your console output for a generated password)

### Endpoints

- `/signin`: Publicly accessible endpoint.
- `/user`: Accessible to users with the `USER` role.
- `/admin`: Accessible to users with the `ADMIN` role.

## Configuration

The security configurations are defined in the `SecurityConfig` class. You can customize it to fit your needs.

- To change the in-memory user details, update the `UserDetailsService` bean in the `SecurityConfig` class.
- To switch to H2 Database authentication, configure the `DataSource` and update the `AuthenticationManagerBuilder`.
