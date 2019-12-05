Esse projeto ilustra a criação de um Microserviço usando o Spring Data Rest.

Swagger/OpenAPI é usado para exemplificar as operações CRUD.

### Exemplo para rodar em Docker

1) Baixar o projeto: 
> git clone

2.1 ) Executar na própria máquina: 

a) Linux ou Mac
> ./mvnw spring-boot:run

b) Windows
> mvnw.cmd spring-boot:run

2.2) Executar em Docker

a) Criar a imagem: 
> docker build -t produtosimg .

b) Rodar aplicação em conteiner: 
> docker run --name produtos -p 8080:8080 -d produtosimg

3) Exemplo de chamada no navegador:
> http://localhost:8080/produtos
> http://localhost:8080/swagger-ui.html
    
### References

* [Official Apache Maven documentation](https://maven.apache.org/guides/index.html)
* [Spring Boot Maven Plugin Reference Guide](https://docs.spring.io/spring-boot/docs/2.2.2.BUILD-SNAPSHOT/maven-plugin/)
* [Spring HATEOAS](https://docs.spring.io/spring-boot/docs/2.2.1.RELEASE/reference/htmlsingle/#boot-features-spring-hateoas)
* [Rest Repositories](https://docs.spring.io/spring-boot/docs/2.2.1.RELEASE/reference/htmlsingle/#howto-use-exposing-spring-data-repositories-rest-endpoint)
* [Spring Data JPA](https://docs.spring.io/spring-boot/docs/2.2.1.RELEASE/reference/htmlsingle/#boot-features-jpa-and-spring-data)
* [Spring Web](https://docs.spring.io/spring-boot/docs/2.2.1.RELEASE/reference/htmlsingle/#boot-features-developing-web-applications)
* [Spring Boot DevTools](https://docs.spring.io/spring-boot/docs/2.2.1.RELEASE/reference/htmlsingle/#using-boot-devtools)

### Guides
The following guides illustrate how to use some features concretely:

* [Building a Hypermedia-Driven RESTful Web Service](https://spring.io/guides/gs/rest-hateoas/)
* [Accessing JPA Data with REST](https://spring.io/guides/gs/accessing-data-rest/)
* [Accessing Neo4j Data with REST](https://spring.io/guides/gs/accessing-neo4j-data-rest/)
* [Accessing MongoDB Data with REST](https://spring.io/guides/gs/accessing-mongodb-data-rest/)
* [Accessing Data with JPA](https://spring.io/guides/gs/accessing-data-jpa/)
* [Building a RESTful Web Service](https://spring.io/guides/gs/rest-service/)
* [Serving Web Content with Spring MVC](https://spring.io/guides/gs/serving-web-content/)
* [Building REST services with Spring](https://spring.io/guides/tutorials/bookmarks/)

