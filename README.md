# Bidding Platform Project
Introduction
This project is a bidding platform that allows users to buy and sell various items through an online marketplace. The platform is designed to facilitate smooth transactions between buyers and sellers, with features such as user authentication, product management, notifications, and real-time chat functionality.

## Features
The project is implemented as six microservices:

### User Service:
Allows users to sign up with OTP verification via Twilio and Redis, manage their profiles, create watchlists, and browse products by category.
### Admin Service:
Provides administrative functionalities such as managing users, products, and categories.
#Product Service:
Handles orders, product listings, and payments. Utilizes cron jobs and Redis for efficient processing.
### Notification Service:
Sends email notifications using RabbitMQ and Gomail library for events such as winning bids and adding items to watchlists.
### Chat Service:
Implements bidirectional streaming for real-time chat between users.
### API Gateway:
Includes authentication with JWT tokens and WebSocket support for chat functionality. Built with Gin framework.

## Technologies Used

* Go (Golang)
* Twilio for OTP verification
* Redis for caching
* RabbitMQ for messaging
* Gomail for email notifications
* WebSocket for chat functionality
* Gin framework for API Gateway
* gRPC for communication between services

## API Documentation
https://documenter.getpostman.com/view/30219361/2sA3JM8MsW
