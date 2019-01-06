Challenge 02 - María José Astudillo Núñez

Métodos de la API REST

Usuarios

El servicio permite manipular datos de usuarios. Los usuarios registrados en la base de datos pueden ingresar al sistema.

Estructura del proyecto

El proyecto sigue la estructura de los proyectos Maven. Por lo tanto, el código fuente Java está ubicado en la carpeta src/main/java dentro del proyecto. El código de la página web está ubicado en la carpeta src/main/

La descripción del API REST se presenta a continuación

	•	CREATE (/users/user): agrega un nuevo usuario a la base de datos.
	•	GET (/users/user): muestra el listado de los usuarios ingresados en la base de datos.
	•	UPDATE (/users/user/{id}): permite modificar la información de un determinado usuario.
	•	DELETE (/users/user/{id}): elimina de forma definitiva a un usuario de la base de datos.

Es posible usar Postman para probar el servicio REST.

	•	Agregar un usuario: POST http://localhost:8080/users/user incluyendo a un usuario en la sección body. Por ejemplo, {“email”: “user@email.com”, “first_name”: “userName”, “last_name” = “userLastName” … }.
	•	Obtener usuarios: GET http://localhost:8080/users /user
	•	Actualizar usuario: PUT http://localhost:8080/users/user/{id} donde id es el valor de id del usuario que se quiere actualizar, y la información nueva se detalla en body. Por ejemplo, usando el ejemplo anterior,  {“email”: “user@email.com”, “first_name”: “userUpdatedName”, “last_name” = “userUpdatedLastName” … }
	•	Eliminar usuario: DELETE http://localhost:8080/users/user/{id} donde id es el valor de id del usuario que se quiere eliminar.

Autos 

El servicio permite manipular datos de autos.

Estructura del proyecto

El proyecto sigue la estructura de los proyectos Maven. Por lo tanto, el código fuente Java está ubicado en la carpeta src/main/java dentro del proyecto. El código de la página web está ubicado en la carpeta src/main/

La descripción del API REST se presenta a continuación

	•	CREATE (/cars/car): agrega un nuevo autos a la base de datos.
	•	GET (/cars/car): muestra el listado de los autos ingresados en la base de datos.
	•	UPDATE (/cars/car/{id}): permite modificar la información de un determinado auto.
	•	DELETE (/cars/car/{id}): elimina de forma definitiva a un auto de la base de datos.

Es posible usar Postman para probar el servicio REST.

	•	Agregar un auto: POST http://localhost:8080/cars/car incluyendo a un usuario en la sección body. Por ejemplo, {“marca”: “Chevrolet”, “modelo”: “Spark”, “color” = “Rojo”}.
	•	Obtener autos: GET http://localhost:8080/cars/car 
	•	Actualizar auto: PUT http://localhost:8080/cars/car/{id} donde id es el valor de id del auto que se quiere actualizar, y la información nueva se detalla en body. Por ejemplo, usando el ejemplo anterior,  {“marca”: “Chevrolet”, “modelo”: “Spark”, “color” = “Verde”}
	•	Eliminar auto: DELETE http://localhost:8080/cars/car/{id} donde id es el valor de id del auto que se quiere eliminar.

Frameworks/Motores utilizados en la aplicación Web

	•	PostgreSQL
	•	Spring Framework
	•	Hibernate
	•	Angular
	•	Bootstrap
	•	Postman
	•	JDBC

Instrucciones para levantar la aplicación

Clonar el repositorio git. Instalar Maven, tener una base de datos PostgreSQL funcionando, y agregar el data source en el archivo application.properties. 

Luego de clonar el repositorio se encontrarán dos carpetas, una corresponde a la aplicación de Spring (portal) y la otra a la aplicación de angular (angular-7-crud). 

Instrucciones para la app. de Spring: 

$ mvn install
$ mvn spring-boot:run

Instrucciones para la app. de Angular:

$ npm install
$ npm install —save @angular-cli/latest
$ ng build
$ ng serve

Ingresar a http://localhost:4200
