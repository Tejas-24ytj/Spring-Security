## Introduction

This project showcases how to integrate Spring Security into a Spring Boot application. It includes examples of authentication, authorization, and various security configurations.

![Screenshot 2024-07-03 174440](https://github.com/Tejas-24ytj/Spring-Security/assets/105742352/58cc50f2-c242-4ce7-bc1c-ba7c474accc5)

![Screenshot 2024-07-03 174723](https://github.com/Tejas-24ytj/Spring-Security/assets/105742352/1012480c-e2bb-4bd3-9c34-eedca9a10724)

![Screenshot 2024-07-03 174944](https://github.com/Tejas-24ytj/Spring-Security/assets/105742352/d784f979-2a83-4c46-afd7-edd398b97237)


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
