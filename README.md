# Proyecto Microservicios con Java, Spring Boot, y Eureka

## Descripción del Proyecto

Este proyecto implementa un sistema de gestión de cursos y estudiantes basado en una arquitectura de microservicios. Utiliza Java, Spring Boot, Eureka, y Spring Cloud Gateway para la gestión y comunicación entre servicios.
  
## Tecnologías usadas

- Java y Spring Boot
- Eureka (Servicio de Registro y Descubrimiento)
- Spring Cloud Gateway (API Gateway)
- Spring Data JPA
- Feign (Cliente Declarativo para Servicios HTTP)
- PostgreSQL y MySQL
- Spring Cloud Config Server (Gestión Centralizada de Configuraciones)

## Estructura del proyecto

Proyecto_Microservicios  
  -├── msvc-config-server  
  -├── msvc-eureka  
  -├── msvc-course  
  -├── msvc-student  
  -├── msvc-gateway

## Habilidades Desarrolladas

 - **Java y Spring Boot:** Desarrollo del backend y gestión de las operaciones de la API.
 - **Arquitectura de Microservicios:** Implementación de servicios independientes y comunicación a través de Eureka y Spring Cloud Gateway.
 - **Spring Cloud Config Server:** Gestión centralizada de configuraciones para todos los microservicios.
 - **Spring Data JPA:** Acceso a bases de datos y gestión de entidades.
 - **Feign:** Cliente declarativo para simplificar las llamadas a servicios HTTP.

## Cómo Clonar y Ejecutar Localmente

1. Abre git bash y clona este repositorio en tu máquina local:
`https://github.com/Porico94/Microservicios.git` 

2. Abre el proyecto en tu IDE preferido (Eclipse, IntelliJ, etc.).

## Consideraciones previas

1. Modificar el archivo msvc-course.yml y msvc-student.yml que se tiene en la carpeta configurations dentro de resources en el microservice.config, que es donde esta centralizado todas las configuraciones, ahí tienes que configurar el puerto, nombre de tu base de datos, username, password y driver. (En este proyecto se está usando MySQL y PostgreSQL).

## Modo de Uso con Postman

1. Acceso a los cursos por Id:
  - Enviar una solicitud GET a http://localhost:8080/api/course/search/id
    ![Captura de Pantalla 1](https://raw.githubusercontent.com/Porico94/Microservicios/master/Capturas%20de%20Pantalla/Captura%20de%20pantalla%20BuscarPorID.png)
    
2. Acceso a todos los cursos:
  - Enviar una solicitud GET a http://localhost:8080/api/course/all
    ![Captura de Pantalla 1](https://raw.githubusercontent.com/Porico94/Microservicios/master/Capturas%20de%20Pantalla/Captura%20de%20pantalla%20TodosLosCursos.png)
    
3. Acceso a los estudiantes por id del curso:
  - Enviar una solicitud GET a http://localhost:8080/api/course/search-student/id
    ![Captura de Pantalla 1](https://raw.githubusercontent.com/Porico94/Microservicios/master/Capturas%20de%20Pantalla/Captura%20de%20pantalla%20BuscarEstudiantePorIdCurso.png)

## Autor

Pool Rimari Córdova
