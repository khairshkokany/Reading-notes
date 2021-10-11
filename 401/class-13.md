# Working with Relationships in Spring Data REST
- One-to-One Relationship
- One-to-Many Relationship
- Many-to-Many Relationship
- Testing the Endpoints With TestRestTemplate

# Integration Testing in Spring

### Spring MVC Test Configuration

- Enable Spring in Tests with JUnit 5
  - JUnit 5 defines an extension interface through which classes can integrate with the JUnit test.


- The WebApplicationContext Object
  - WebApplicationContext provides a web application configuration. It loads all the application beans and controllers into the context.

- Mocking Web Context Beans
  - MockMvc provides support for Spring MVC testing. It encapsulates all web application beans and makes them available for testing.

- Verify Test Configuration

### Writing Integration Tests

- Verify View Name
- Verify Response Body
- Send GET Request With Path Variable
- Send GET Request With Query Parameters
- Send POST Request

### MockMvc Limitations
- MockMvc provides an elegant and easy-to-use API to call web endpoints and to inspect and assert their response at the same time. Despite all its benefits, it has a few limitations.

- First of all, it does use a subclass of the DispatcherServlet to handle test requests. To be more specific, the TestDispatcherServlet is responsible for calling controllers and performing all of the familiar Spring magic.

- The MockMvc class wraps this TestDispatcherServlet internally. So, every time we send a request using the perform() method, MockMvc will use the underlying TestDispatcherServlet directly. Therefore, there are no real network connections made, and consequently, we won't test the whole network stack while using MockMvc.

- Also, because Spring prepares a fake web application context to mock the HTTP requests and responses, it may not support all features of a full-blown Spring application.
