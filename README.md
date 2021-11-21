🎥 **Cinema Service** 🎥
-

This is a simulation of the cinema service with the ability to create a hall, movies, sessions, tickets, users and their orders. The capabilities of the user are determined by his role(user, admin).

**How start using**

To test the site you can enter the account as a user 
using the login: user@i.ua with the password: user123
or as an administrator - admin@i.ua, admin123
**link:** http://

To go through the pages of the site you need to change the request address.

Typical queries:

- POST: /register, /login, /logout
- GET: /cinema-halls, POST: /cinema-halls, /movie-sessions, /movies, /movie-sessions/available?movieId&date, /shopping-carts/by-user, /orders, /users/by-email?email
- POST: /cinema-halls, /movie-sessions, /movies, /movie-sessions, /movie-sessions/{id}, /orders/complete
- PUT: /shopping-carts/movie-sessions?movieSessionId

**Note:** Some post requests can only be thrown when you are authorized as an administrator and used to update or change the information in the database. Use a postman or its analogue for this purpose.

**How to configure java code for your database?**
- Fork repository
- To get started, you need to replace the database data in the folder: src/main/resources/db.properties
- If you are using a database other than mySql you need to change the dependency in the pom.xml file
- Use tomcat or its analogues to run the application

**Technologies used:**

- JDK 11
- Spring Web
- Spring Security
- Spring ORM
- Hibernate 
- Servlet API
- Maven
- JSON
- Tomcat

**Recommended software**
1. Intellij idea
2. jdk 11
3. MySQL
4. Tomcat 9.0.54
