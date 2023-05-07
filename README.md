<h1 align="center"> Employees_Address </h1>

>## Database
* [MySQL](https://www.mysql.com/downloads/)

>## Framework 
* [SpringBoot](javatpoint.com/spring-boot-tutorial)

>## Language 
* [Java](https://www.java.com/en/download/help/whatis_java.html)

>## Data flow
In this project, we have 4 layers-
* **Controller** - The controller layer handles the HTTP requests, translates the JSON parameter to object, and authenticates the request and transfer it to the business (service) layer.
* **Service** -The business layer handles all the business logic. It consists of service classes and uses services provided by data access layers.
* **Repository** - This layer mainatains the h2-database thing on which CRUD operations are performed
* **Model** - This layer consists basically the class level things- the various classes required for the project and these classes consists the attributes to be stored.

>## API Documentation
The following APIs are provided by the application:

Employee APIs
* GET- /employees - get all employees
* GET- /employees/{id} - get an employee by id
* POST-   /employees - create a new employee
* PUT-    /employees/{id} - update an employee by id
* DELETE- /employees/{id} - delete an employee by id

Address APIs
* GET- /addresses - get all addresses
* GET- /addresses/{id} - get an address by id
* POST- /addresses - create a new address
* PUT- /addresses/{id} - update an address by id
* DELETE- /addresses/{id} - delete an address by id

### Request and Response Formats
The APIs expect and return data in JSON format. Here are some examples:


```
[
    {
        "id": 1,
        "firstName": "Saeed",
        "lastName": "Mujawar",
        "address": {
            "id": 1,
            "street": "23 Line colony",
            "city": "Miraj",
            "state": "Maharashtra",
            "pincode": "416410"
        }
    },
    {
        "id": 2,
        "firstName": "Saad",
        "lastName": "Mujawar",
        "address": {
            "id": 2,
            "street": "mendhe plot st",
            "city": "Sangli",
            "state": "Maharashtra",
            "zipcode": "416410"
        }
    }
]

```

>## Project Summary
This project demonstrates the basic usage of Spring Boot and Hibernate to build a RESTful API for managing employees and addresses.