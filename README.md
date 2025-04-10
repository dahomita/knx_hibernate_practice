# Bookstore Application

This is a Spring Boot application that provides a RESTful API for managing bookstore data. The application comes with integrated Swagger UI for exploring and testing the CRUD endpoints.

## Prerequisites

Before running the application, please ensure you have the following installed:

- **Java 11 (or later)**: Make sure Java is installed and your `JAVA_HOME` environment variable is set.
- **MySQL**: Install MySQL to manage the database.
- **Maven**: Although the project includes the Maven Wrapper, having Maven installed can be useful.

## Database Setup

1. **Install MySQL:**  
   If you haven't already, install MySQL from [MySQL Downloads](https://dev.mysql.com/downloads/mysql/).

2. **Create the Database:**  
   Open your MySQL client and create a new database named `bookstore`. The application uses the following connection URL:jdbc:mysql://localhost:3306/bookstore
   
3. **Configure Credentials:**  
Update the database username and password in the application's configuration file (`src/main/resources/application.properties` or `application.yml`) if necessary. For example:

```
properties
spring.datasource.url=jdbc:mysql://localhost:3306/bookstore
spring.datasource.username=your_username
spring.datasource.password=your_password
spring.datasource.driver-class-name=com.mysql.cj.jdbc.Driver
 ```                                                                                                                
                                                                                                                      
                                                                                                                                                                                                                                       
## Running the Application
   To run the application, use the Maven Wrapper provided in the repository. Execute the following command from the project root directory:
   ```
   ./mvnw spring-boot:run
   ``` 
   