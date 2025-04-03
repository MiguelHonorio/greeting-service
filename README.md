# Getting Started

## Ferramentas necessárias

- JDK 17
- IDE de sua preferência

### Documentação de referência
Para mais informações, consulte as seguintes secções:

* [Official Apache Maven documentation](https://maven.apache.org/guides/index.html)
* [Spring Boot Maven Plugin Reference Guide](https://docs.spring.io/spring-boot/3.4.1/maven-plugin)
* [Create an OCI image](https://docs.spring.io/spring-boot/3.4.1/maven-plugin/build-image.html)
* [Spring Web](https://docs.spring.io/spring-boot/3.4.1/reference/web/servlet.html)
* [Spring Boot Actuator](https://docs.spring.io/spring-boot/3.4.1/reference/actuator/index.html)
* [Config Client](https://docs.spring.io/spring-cloud-config/reference/client.html)

### Guias
Os guias seguintes ilustram a utilização concreta de algumas funcionalidades:

* [Building a RESTful Web Service](https://spring.io/guides/gs/rest-service/)
* [Serving Web Content with Spring MVC](https://spring.io/guides/gs/serving-web-content/)
* [Building REST services with Spring](https://spring.io/guides/tutorials/rest/)

#### Spring Actuator
O Spring Actuator fornece todos os recursos necessários para monitor e gerenciar a aplicação.
* [Building a RESTful Web Service with Spring Boot Actuator](https://spring.io/guides/gs/actuator-service/)


### Substituições do Maven Parent

Devido ao design do Maven, os elementos são herdados do POM pai para o POM do projeto.
Embora a maior parte da herança seja boa, ela também herda elementos indesejados como `<license>` e `<developers>` do pai.
Para evitar isso, o POM do projeto contém overrides vazios para esses elementos.
Se você mudar manualmente para um pai diferente e realmente quiser a herança, você precisa remover esses overrides.
