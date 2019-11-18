# SpringBootDemo
 A demo to create a Web API using Spring Boot

This demo follows the implementation given by Amigos Code's tutorial, found [here](https://www.youtube.com/watch?v=vtPkZShrvXQ).

#How To Run
1. Navigate into repository folder in terminal
2. java -jar .\demo-0.0.1-SNAPSHOT.jar

#How To Use
1. By using a tool like Postman, you can make API requests to port 8080 at this URI: localhost:8080/api/v1/person
- The user can get a list of all people in the database by sending a GET to localhost:8080/api/v1/person
- The user can get a specifific person by id in the database by sending a GET to localhost:8080/api/v1/person/**insert id**
- The user can add People to the in-memory database by sending a POST to localhost:8080/api/v1/person with a JSON body containing the name:
```json
{
	"name": "Richard Hendricks"
}
```
- The user can change the name of a person by id by sending a PUT to localhost:8080/api/v1/person/**insert id** with a JSON body containing the new name:
```json
{
	"name": "Gavin Belson"
}
```
- The user can delete a person by id from the database by sending a DELETE to localhost:8080/api/v1/person/**insert id**