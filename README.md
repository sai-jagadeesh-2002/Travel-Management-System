# Travel-Management-System

## Overview

This documentation provides comprehensive information about the Travel Booking System Database. This system manages flights, hotels, car rentals, customer reservations, payments, and trip itineraries.

## Implemented Features

1. **Database Schema**: The database consists of various tables, including `Guest` and `Hotel`, which store information about guests and hotels, respectively.

2. **Endpoints**:
    - **Guest Endpoints**:
        - `GET /api/v1/guests`: Retrieve all guests.
        - `GET /api/v1/guests/{id}`: Retrieve details of a specific guest.
        - `POST /api/v1/guests`: Create a new guest.
        - `PUT /api/v1/guests/{id}`: Update details of an existing guest.
        - `DELETE /api/v1/guests/{id}`: Delete a guest.
    - **Hotel Endpoints**:
        - `GET /api/v1/hotels`: Retrieve all hotels.
        - `GET /api/v1/hotels/{id}`: Retrieve details of a specific hotel.
        - `POST /api/v1/hotels`: Create a new hotel.
        - `PUT /api/v1/hotels/{id}`: Update details of an existing hotel.
        - `DELETE /api/v1/hotels/{id}`: Delete a hotel.
   
3. **Security**: Endpoints are secured using JWT (JSON Web Token) authentication. Only authenticated users can access the endpoints.

4. **Documentation**: Swagger/OpenAPI documentation is available to understand and explore the API endpoints.

5. **Logging**: SLF4J or Log4j is implemented to log application events and errors for monitoring and troubleshooting purposes.

### How to Use

#### Using the Endpoints

1. Ensure that the application is running.
2. Use an HTTP client tool like Thunderclient, Postman or cURL to interact with the endpoints.
3. Send requests to the appropriate endpoints using the specified HTTP methods (GET, POST, PUT, DELETE).
4. Include the necessary request parameters and payload in the request body where required.
5. Authenticate the requests with a valid JWT token to access secured endpoints.

#### Accessing Swagger Documentation

1. Once the application is running, navigate to the Swagger UI documentation page.
2. The Swagger UI page typically resides at `/swagger-ui.html` or `/swagger-ui/index.html`.
3. Explore the available endpoints, request parameters, and response structures using the Swagger UI interface.
4. Test the endpoints directly from the Swagger UI by providing input parameters and observing the responses.

### Sample Requests

#### Retrieve All Guests

- **Request**: `GET /api/v1/guests`
- **Response**: Returns a list of all guests with their details.

#### Create a New Guest

- **Request**: `POST /api/v1/guests`
- **Request Body**: Provide the necessary details of the new guest.
- **Response**: Returns the details of the newly created guest along with a success message.

#### Update Guest Details

- **Request**: `PUT /api/v1/guests/{id}`
- **Request Body**: Provide the updated details of the guest.
- **Response**: Returns the updated details of the guest along with a success message.

#### Delete a Guest

- **Request**: `DELETE /api/v1/guests/{id}`
- **Response**: Deletes the specified guest and returns a success message.

### Conclusion

This documentation provides a comprehensive overview of the Travel Booking System Database, including its features, endpoints, security measures, and usage instructions. Use this guide to effectively utilize the system's functionalities for managing flights, hotels, and customer reservations.
