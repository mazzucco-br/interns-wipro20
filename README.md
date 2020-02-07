# interns-wipro20

## users-api
Identity Microservice to make operations related to Users
<pre>
api  
  users
    create (POST /users)
      UserCreateControler
      UserCreateService
      UserCreateRequest
      UserCreateResponse
    update (PUT /users/{id})
    detail (GET /users/{id})
    list (GET /users) - filter and pagination
    delete (DELETE /users/{id})
  roles
    create
      RoleCreateControler
      RoleCreateService
      RoleCreateRequest
      RoleCreateResponse
    update
    detail
    list
    delete
domain
  user
    User
    UserRepository    
  role
    Role
      id
      name
    RoleRepository
</pre>

## logs-api
Log Microservice to write logs received through the API
<pre>
api
  logs
    create
    search
</pre>    

## TODO
<pre>

- integration tests (rest) with SpringBoot
- success tests
	- validate status code 200
- fail tests
	- validate status code 400
	- validate error messages for each field that has not been informed

Log all events to log microservice
  - Interface Logable
H2DB - memory database
Swagger
Generate RequestId
Add user_id to header
BeanValidation
  add validations for each field or the request object
  reference: https://docs.oracle.com/javaee/6/tutorial/doc/gircz.html
ExceptionHandling 
Security
</pre>

