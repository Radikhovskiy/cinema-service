🎥 **Cinema Service** 🎥
-

This is a simulation of the cinema service with the ability to create a hall, movies, sessions, tickets, users and their orders. The capabilities of the user are determined by his role(user, admin).

**How start using**

To test the site you can enter the account as a user 
using the login: user@i.ua with the password: user123
or as an administrator - admin@i.ua, admin123

**link:** http://cinema-radik.herokuapp.com/login

List of endpoints::

- POST: /register, /login (all)
- GET: /orders, /orders/complete, /shopping-carts/by-user (user), /cinema-halls, /cinema-halls, /movie-sessions, /movies, /movie-sessions/, available?movieId&date, /logout (user/admin) /users/by-email?email (admin)
- POST: /cinema-halls, /movie-sessions, /movies, /movie-sessions, /movie-sessions/{id}, /orders/complete (admin)
- PUT: /shopping-carts/movie-sessions?movieSessionId (admin)

**Note:** Some post requests can only be thrown when you are authorized as an administrator and used to update or change the information in the database. Use a postman or its analogue for this purpose.

**Setup**
- Fork repository
- Replace the database data in the folder: src/main/resources/db.properties
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
- Tomcat

**Recommended software**
1. Intellij idea
2. jdk 11
3. MySQL
4. Tomcat 9.0.54
