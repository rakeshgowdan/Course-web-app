##Full Stack CRUD application with React and Spring Boot  
##Important points to note:

REST API is exposed using Spring Boot
REST API is consumed from React Frontend to present the UI
The Database, in this example, is a hardcoded in-memory static list.

##Getting an overview of Spring Boot REST API Resources
In this guide, we will create these services using proper URIs and HTTP methods:

@GetMapping("/instructors/{username}/courses") : Get Request Method exposing the list of courses taught by a specific instructor
@GetMapping("/instructors/{username}/courses/{id}") : Get Request Method exposing the details of a specific course taught by a specific instructor
@DeleteMapping("/instructors/{username}/courses/{id}") : Delete Request Method to delete a course belonging to a specific instructor
@PutMapping("/instructors/{username}/courses/{id}") : Put Request Method to update the course details of a specific course taught by a specific instructor
@PostMapping("/instructors/{username}/courses") : Post Request Method to create a new course for a specific instructor

""The REST API can be enhanced to interact with other microservices infrastructure components and act as microservices.""