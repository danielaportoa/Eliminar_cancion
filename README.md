Proyecto Canciones
Este repositorio contiene una aplicación web completa desarrollada en Java con el framework Spring Boot. Implementa de manera estricta el patrón arquitectónico MVC (Modelo-Vista-Controlador) y utiliza Spring Data JPA junto con Hibernate para gestionar operaciones CRUD completas en una base de datos relacional MySQL.

El diseño del sistema permite listar un catálogo, examinar el detalle individual de cada registro, agregar nuevas canciones mediante validaciones del lado del servidor y actualizar características existentes simulando verbos HTTP avanzados.
---
Objetivos del Proyecto Cumplidos
Arquitectura MVC Dinámica
Validación en el Servidor
Soporte de Métodos Ocultos
Estilos Centralizados
---
Tecnologías Utilizadas
Java 17
Spring Boot 3.2.x / 3.3.x
Spring Boot Starter Validation
Spring Data JPA & Hibernate
MySQL Connector / J
Apache Tomcat (Embed)
JSTL (Jakarta Standard Tag Library) & Spring Form Tags
Maven
---
Estructura de Archivos del Proyecto
canciones/
├── src/
│   ├── main/
│   │   ├── java/
│   │   │   └── com/cl/
│   │   │       ├── CancionesApplication.java  
│   │   │       ├── controladores/           
│   │   │       ├── modelos/                  
│   │   │       ├── repositorios/             
│   │   │       └── servicios/                
│   │   ├── resources/
│   │   │   ├── static/
│   │   │   │   └── estilos.css               
│   │   │   └── application.properties        
│   │   └── webapp/
│   │       └── WEB-INF/                      
│   │           ├── canciones.jsp            
│   │           ├── detalleCancion.jsp        
│   │           ├── agregarCancion.jsp        
│   │           └── editarCancion.jsp         
└── pom.xml                                  
