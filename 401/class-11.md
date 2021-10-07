## Starting with Spring Initializr

![image spring](https://media.geeksforgeeks.org/wp-content/uploads/Spring-Framework-Architecture.png)

- visit the Spring Initializr to generate a new project with the required dependencies (Spring Web, Thymeleaf, and Spring Boot DevTools).
- Create a Web Controller.

  - In Spring’s approach to building web sites, HTTP requests are handled by a controller. You can easily identify the controller by the @Controller annotation.

  - The implementation of the method body relies on a view technology to perform server-side rendering of the HTML.

- Spring Boot Devtools

  - A common feature of developing web applications is coding a change, restarting your application, and refreshing the browser to view the change. This entire process can eat up a lot of time. To speed up this refresh cycle, Spring Boot offers with a handy module known as spring-boot-devtools.

- Run the Application

  - The Spring Initializr creates an application class for you. In this case, you need not further modify the class provided by the Spring Initializr.


---

- Spring model attributes

  - Spring MVC calls the pieces of data that can be accessed during the execution of views model attributes. The equivalent term in Thymeleaf language is context variables.

- Request parameters

  - Request parameters can be easily accessed in Thymeleaf views. Request parameters are passed from the client to server.


- Session attributes

  - Similarly to the request parameters, session attributes can be accessed by using the session. 


- ServletContext attributes

  - The ServletContext attributes are shared between requests and sessions. In order to access ServletContext attributes in Thymeleaf you can use the #servletContext.

- Spring beans

  - Thymeleaf allows accessing beans registered at the Spring Application Context with the @beanName syntax.