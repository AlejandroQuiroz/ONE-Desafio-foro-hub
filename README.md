# ForoHub

**ForoHub** es una API REST desarrollada con Spring Framework para gestionar un foro de discusión. Los usuarios pueden crear, leer, actualizar y eliminar tópicos (CRUD). La API está diseñada siguiendo las mejores prácticas del modelo REST, e incluye validaciones, autenticación/autorización y una base de datos relacional para la persistencia de la información.

## Características

- Crear un nuevo tópico
- Mostrar todos los tópicos creados
- Mostrar un tópico específico
- Actualizar un tópico
- Eliminar un tópico
- Validaciones de las reglas de negocio
- Autenticación y autorización de usuarios

## Tecnologías Utilizadas

- **Java 17**
- **Spring Boot**
- **Spring Data JPA**
- **Spring Security**
- **Hibernate**
- **Postgres**
- **Maven**

## Instalación y Ejecución

### Prerrequisitos

- JDK 17 o superior
- Maven
- Postgres

### Configuración

**Configurar la base de datos**:

- Actualizar las configuraciones en `src/main/resources/application.yml` con las credenciales de tu base de datos.

    ```properties
    url: jdbc:postgresql://localhost:5432/<tu-db>
    username: <tu-usuario>
    password: <tu-password>
    ```

### Autenticación y Autorización

La API usa **Spring Security** para la autenticación y autorización. Los usuarios deben autenticarse para acceder a los endpoints. 

### Validaciones

- Todos los campos son obligatorios al crear o actualizar un tópico.
- Los mensajes de error se devuelven en caso de fallos en las validaciones.