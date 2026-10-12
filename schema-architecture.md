Smart Clinic Management System Architecture
1. Architecture Summary :
   
The Smart Clinic Management System follows a three-tier architecture consisting of the Presentation Layer, Application Layer, and Data Layer. Users interact with the system through web pages developed using Thymeleaf or through REST APIs. The Application Layer, built with Spring Boot, processes user requests using controllers and services that implement business logic. Data is stored and retrieved using two databases: MySQL for relational data through Spring Data JPA and MongoDB for document-based data through Spring Data MongoDB. This architecture promotes scalability, maintainability, and separation of concerns.

3. Numbered Flow :
   
The user accesses the Smart Clinic Management System through a web browser or API client.
The Presentation Layer displays web pages using Thymeleaf templates or accepts REST API requests.
The user submits a request, such as registering a patient or booking an appointment.
The request is received by a Spring MVC Controller or REST Controller.
The controller passes the request to the appropriate Service Layer component.
The Service Layer validates the request and applies business rules.
The application accesses MySQL through Spring Data JPA to manage structured clinic data.
The application accesses MongoDB through Spring Data MongoDB to manage document-oriented data.
The database returns the requested information or confirms the transaction.
The Service Layer processes the database response.
The controller prepares the final response.
The response is returned as an HTML page or REST API response to the user.
