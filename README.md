# Proyecto Canciones - Spring Boot CRUD MVP 

Este repositorio contiene una aplicación web completa desarrollada en **Java** con el framework **Spring Boot**. 
Implementa de manera estricta el patrón arquitectónico **MVC (Modelo-Vista-Controlador)** y utiliza **Spring Data JPA** junto con **Hibernate** para gestionar operaciones CRUD completas en una base de datos relacional **MySQL**.

El diseño del sistema permite listar un catálogo, examinar el detalle individual de cada registro, agregar nuevas canciones mediante validaciones del lado del servidor y actualizar características existentes simulando verbos HTTP avanzados.

---

## Objetivos 

* **Arquitectura MVC Dinámica** 
* **Validación en el Servidor** 
* **Soporte de Métodos Ocultos** 
* **Estilos Centralizados** 
---

## Tecnologías Utilizadas

* **Java 17** 
* **Spring Boot 3.2.x / 3.3.x**
* **Spring Boot Starter Validation** 
* **Spring Data JPA & Hibernate**
* **MySQL Connector / J**
* **Apache Tomcat (Embed)** 
* **JSTL (Jakarta Standard Tag Library) & Spring Form Tags**
* **Maven** 

---

## Estructura de Archivos del Proyecto

```text
canciones/
├── src/
│   ├── main/
│   │   ├── java/
│   │   │   └── com/cl/
│   │   │       ├── CancionesApplication.java  # Clase principal de arranque
│   │   │       ├── controladores/            # Controladores que mapean rutas GET, POST, PUT
│   │   │       ├── modelos/                  # Objeto de dominio (@Entity) y reglas @Size
│   │   │       ├── repositorios/             # Interfaz de datos (CrudRepository)
│   │   │       └── servicios/                # Lógica de negocio (agregar, buscar, actualizar)
│   │   ├── resources/
│   │   │   ├── static/
│   │   │   │   └── estilos.css               # Hoja de estilos centralizada y homogenizada
│   │   │   └── application.properties        # Configuración de BD y filtros mvc
│   │   └── webapp/
│   │       └── WEB-INF/                      # Directorio seguro de vistas JSP
│   │           ├── canciones.jsp             # Catálogo principal con vista de tabla
│   │           ├── detalleCancion.jsp        # Ficha de detalle con botones de acción y fechas
│   │           ├── agregarCancion.jsp        # Formulario de inserción con renderizado de errores
│   │           └── editarCancion.jsp         # Formulario de modificación precargado (PUT)
└── pom.xml                                   # Declaración de dependencias del proyecto
