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
<pre>
- testes de integração (rest) com SpringBoot
- um teste sucesso
	- validar status code 200
- um teste de erro com nenhum campo informado
	- validar status code 400
	- validar mensagem para cada campo requerido

Log all events to log microservice
  - Interface Logable
H2DB - configurar banco de memória
Swagger
Generate RequestId
Add user_id to header
BeanValidation
  adicionar validações para os campos de requisição
  vide https://docs.oracle.com/javaee/6/tutorial/doc/gircz.html
ExceptionHandling 
Security
</pre>

