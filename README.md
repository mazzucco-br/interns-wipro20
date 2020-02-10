# interns-wipro20

## users-api
Identity Microservice to make operations related to Users
<pre>
api  
  users
    common
      UsersMapper
        User toUsers(UsersDto user);
	UsersDto toUsersDto(User user);
      UsersDto
        id
        email
        firstName
        lastName
        birthDate
        roles
    create (POST /users)
      UsersCreateController
      UsersCreateService
      UsersCreateRequest extends UsersDto
      UsersCreateResponse extends UsersDto
    update (PUT /users/{id})
      UsersUpdateController
      UsersUpdateService
      UsersUpdateRequest extends UsersDto
      UsersUpdateResponse extends UsersDto
    detail (GET /users/{id})
      UsersDetailController
      UsersDetailService
      UsersDetailResponse extends UserDto
    list (GET /users) - filter and pagination
    delete (DELETE /users/{id})
  roles
    create (POST /roles)
      RoleCreateController
      RoleCreateService
      RoleCreateRequest
      RoleCreateResponse
    update (PUT /roles/{id})
    detail (GET /roles/{id})
    list (GET /roles)
    delete (DELETE /roles/{id})
domain
  user
    User
      id
      email
      firstName
      lastName
      birthDate
      roles
    UserRepository
  role
    Role
      id
      name
    RoleRepository
common
  exception
</pre>

## logs-api
Log Microservice to write logs received through the API
<pre>
api
  logs
    create (POST /logs)
    search (POST /logs/search)
      LogsSearchRequest
        queryParams
	  field
	  value
	
	
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

