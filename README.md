# Spring Demo Example

### Basic
*https://spring.io/quickstart*

- **@RestController** ...annotation tells Spring that this code describes an endpoint that should be made available over the web.

- **@GetMapping(“/hello”)** ... tells Spring to use hello() method to answer requests that get sent to the http://localhost:8080/hello address.

- **@RequestParam** ...tells Spring to expect a name value in the request, but if it’s not there, it will use the word “World” by default.

### Rest - Service

*https://spring.io/guides/gs/rest-service/*

1. **Resource Representation Class** ...`Greeting.java`

1. **Resource Controller** ...Spring approach to build RESTful web services: *HTTP requests are handled by a controller* 
    
    - **@RestController** ...marks the class as a controller where every method returns a domain object instead of a view. It is shorthand for including both **@Controller** and **@ResponseBody** 
    
    - **@GetMapping** ...ensures that HTTP GET requests to /greeting are mapped to the greeting() method. ALternative: @RequestMaping(method=GET)
    
    - **@RequestParam** ...binds the value of the query string parameter name into the name parameter of the greeting() method
    
   