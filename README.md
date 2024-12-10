# Microservice for user registration, login, and profile management in UMass Hangout


User Registration Service API
The User Registration Service manages user account operations, including signing up for new accounts, logging in to existing accounts, and managing user profiles. It provides the following REST endpoints:

/api/v1/auth/register: Enables new user registration. Throws an error if the email ID is already registered.

/api/v1/auth/login: Authenticates users with valid credentials. Suggests signing up if no account exists for the provided email ID.

/api/v1/auth/profile/{emailId}: Retrieves profile information for the specified email ID. Throws an error if no account is found.

/api/v1/auth/profile: Creates or updates a user profile. Throws an error if the associated account does not exist.

Tech Stack Used:

All required depedencies are part of pom.xml

Programming Language - Java  - 1.8

Framework - Spring boot - 2.5.5

Database - MySQL database

Testing - JUnit/Mockito

Steps to run:
Clone the repo
Run the application
The service is set to run on port 8080. please change server.port in application.properties if needed
