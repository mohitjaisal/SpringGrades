<div align="center">
  <img src="https://raw.githubusercontent.com/mohitjaisal/SpringGrades/master/src/main/resources/static/logo.png" alt="Spring Grades Logo" width="60%" height="auto" />
<br/>
  <p>
    This is a simple student grades system built using Spring Boot framework. The application follows a three-layer code base architecture and utilizes Thymeleaf for server-side rendering and MVC (Model-View-Controller) design pattern for handling user requests and responses.
  </p>
</div>

### Installation
To run the student grades system locally, follow these steps:

- Clone the repository:
```
git clone https://github.com/mohitjaisal/student-grades-system.git
```

- Navigate to the project directory:
```
cd student-grades-system
```

- Build the project using Maven:
```
mvn clean install
```


Student Grades System
This is a simple student grades system built using Spring Boot framework. The application follows a three-layer code base architecture and utilizes Thymeleaf for server-side rendering and MVC (Model-View-Controller) design pattern for handling user requests and responses.

Installation
To run the student grades system locally, follow these steps:

Clone the repository:

bash
Copy code
git clone https://github.com/your-username/student-grades-system.git
Navigate to the project directory:

bash
Copy code
cd student-grades-system
Build the project using Maven:

bash
Copy code
mvn clean install
Run the application:

bash
Copy code
mvn spring-boot:run
Open your web browser and visit http://localhost:8080 to access the student grades system.

### Technologies Used
The student grades system is built using the following technologies:

<b>Spring Boot:</b> A popular Java framework for building web applications.
<b>Thymeleaf:</b> A server-side Java template engine for rendering HTML.
<b>MVC (Model-View-Controller):</b> A design pattern for structuring web applications.

### Project Structure
The project follows a three-layer code base architecture, which helps in maintaining a clear separation of concerns and improves code organization. The layers are as follows:

<b>Controller Layer:</b> Handles user requests and responses, and acts as an interface between the user and the application. This layer is responsible for processing inputs, invoking the appropriate services, and returning the results to the user.

<b>Service Layer:</b> Contains the business logic of the application. It performs operations such as data validation, calculations, and interactions with the data access layer.

<b>Data Access Layer:</b> Handles data persistence and retrieval. It communicates with the database or any other data source to perform CRUD (Create, Read, Update, Delete) operations.

Run the application:
```
mvn spring-boot:run
```

Open your web browser and visit http://localhost:8080 to access the student grades system.

### Thymeleaf
Thymeleaf is a server-side Java template engine that allows you to build dynamic web pages. It seamlessly integrates with Spring Boot and provides powerful features such as expression language, iteration, conditional statements, and form handling.

To use Thymeleaf in your Spring Boot project, follow these steps:

- Add the Thymeleaf dependency to your project's pom.xml file:

```
<dependency>
    <groupId>org.springframework.boot</groupId>
    <artifactId>spring-boot-starter-thymeleaf</artifactId>
</dependency>
```

- Configure Thymeleaf in your Spring Boot application properties (e.g., `application.properties`):
```
spring.thymeleaf.enabled=true
```

- Create Thymeleaf templates (HTML files) in the appropriate directory (e.g., src/main/resources/templates).

Use Thymeleaf expressions and tags in your templates to dynamically render data and handle user interactions.

### MVC (Model-View-Controller)
MVC is a design pattern that separates the concerns of an application into three components: the Model, the View, and the Controller.

<b>Model:</b> Represents the data and business logic of the application. It interacts with the data access layer to perform CRUD operations.

<b>View:</b> Represents the user interface of the application. It renders the data provided by the controller and handles user interactions.

<b>Controller:</b> Handles user requests, processes input, and determines the appropriate response. It interacts with the service layer to perform business operations and provides data to the view.

<b>To implement MVC in your Spring Boot application:</b>

- Create model classes to represent your data entities.

- Create controller classes and annotate them with `@Controller` to mark them as request handlers.

- Use appropriate annotations (`@RequestMapping, @GetMapping, @PostMapping, etc.`) to map URLs to controller methods.

- Create service classes to encapsulate the business logic and annotate them with @Service.

- Use appropriate annotations (`@Autowired, @Valid, etc.`) to inject dependencies and perform data validation.

- Create Thymeleaf templates (`views`) to render data and handle user interactions.

- Connect the layers by invoking appropriate methods and passing data between them.

### Validation Annotations
Spring provides several annotations for data validation in the controller layer. Some commonly used annotations are:

`@NotNull:` Validates that the annotated field is not null.

`@NotEmpty:` Validates that the annotated field is not empty.

`@NotBlank:` Validates that the annotated field is not null and the trimmed length is greater than zero.

`@Min:` Validates that the annotated field is a number and its value is greater than or equal to the specified minimum value.

`@Max:` Validates that the annotated field is a number and its value is less than or equal to the specified maximum value.

`@Pattern:` Validates that the annotated field matches the specified regular expression pattern.


You can use these annotations to ensure data integrity and enforce validation rules in your application.


<b>Note:</b> Don't forget to include the necessary dependencies for validation in your pom.xml file and configure them appropriately in your Spring Boot application.

This is a basic overview of the student grades system, Thymeleaf, the three-layer code base architecture, and the use of MVC and validation annotations in Spring Boot. Feel free to explore these concepts further and customize the implementation based on your requirements.
