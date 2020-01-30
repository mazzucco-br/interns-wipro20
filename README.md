# interns-wipro20

## users-api
<pre>
api  
  user
    create (POST /users)
      UserCreateControler
      UserCreateService
      UserCreateRequest
      UserCreateResponse
    update (PUT /users/{id})
    detail (GET /users/{id})
    list (GET /users) - filter and pagination
    delete (DELETE /users/{id})
  role
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
    RoleRepository
## logs-api    
api
  log
    create
    search
</pre>
## TODO
Log all events to log microservice
  - Interface Logable
H2DB
Swagger
RequestId
Add user_id header
BeanValidation
ExceptionHandling 
Security


