# Spring Authentication 

![image](https://i.ytimg.com/vi/pVxiB4gC7P4/maxresdefault.jpg)

## Authentication and Access Control

- Authentication (who are you?) and Authorization (what are you allowed to do?)

## Authentication
- The main strategy interface for authentication is AuthenticationManager, which has only one method:

public interface AuthenticationManager {

  Authentication authenticate(Authentication authentication)
    throws AuthenticationException;
}
- An AuthenticationManager can do one of 3 things in its authenticate() method:

  - Return an Authentication (normally with authenticated=true) if it can verify that the input represents a valid principal.

  - Throw an AuthenticationException if it believes that the input represents an invalid principal.

  - Return null if it cannot decide.


- The most commonly used implementation of AuthenticationManager is ProviderManager, which delegates to a chain of AuthenticationProvider instances. 


## Authorization or Access Control

- There are three implementations provided by the framework and all three delegate to a chain of AccessDecisionVoter instances, a bit like the ProviderManager delegates to AuthenticationProviders.

## Web Security
![image_Network](https://bs-uploads.toptal.io/blackfish-uploads/blog/common_mistakes_guide/content/cover_image_file/cover_image/16704/cover-Redesign-WebSecurityVulnerabilities-Luke_Newsletter-04d5cdafdaf363f0bc6aa723a391c343-91ee4d294318c967b26187f4d67a8351.png)

- Spring Security in the web tier (for UIs and HTTP back ends) is based on Servlet Filters, so it is helpful to first look at the role of Filters generally

- The client sends a request to the application, and the container decides which filters and which servlet apply to it based on the path of the request URI.

## Combining Application Security Rules with Actuator Rules


- If you want your application security rules to apply to the actuator endpoints, you can add a filter chain that is ordered earlier than the actuator one and that has a request matcher that includes all actuator endpoints.

