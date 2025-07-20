Section 1
This Spring Boot application uses both MVC and REST controllers. Thymeleaf templates are used for the Admin and Doctor dashboards, 
while REST APIs serve all other modules. The application interacts with two databases—MySQL (for patient, doctor, appointment, and admin data) 
and MongoDB (for prescriptions). All controllers route requests through a common service layer, which in turn delegates to the appropriate repositories. 
MySQL uses JPA entities while MongoDB uses document models.


Section 2
1. User accesses AdminDashBoard or Appointment pages.
2. The action is routed to the appropriate Thymeleaf or REST controller.
3. Controller calls the service layer to execute the logic.
4. Service layer will retrieve any data required from repositories.
5. Repositories are query data from databases.
6. Models are binded to Database.
7. Application Models 
