# Gestor-deportes-acuaticos

# Reto-5-Práctica-01
Generar la documentación en Markdaown del proyecto que estáis realizando en el módulo de Programación.

1. Descripción del proyecto
El Gestor de Deportes Acuáticos es una aplicación desarrollada en JavaFX con conexión a MySQL, diseñada para gestionar usuarios, reservas y actividades relacionadas con deportes acuáticos.

El sistema permite registrar clientes, empleados y administradores, gestionar reservas y visualizar actividades disponibles.
Este proyecto se ha desarrollado como práctica del módulo de Programación del ciclo formativo de Desarrollo de Aplicaciones Multiplataforma (DAM).

2. Tecnologías utilizadas
Java 17

JavaFX 17

MySQL 8

JDBC

CSS

Scene Builder

Visual Studio Code

3. Estructura del código
El proyecto sigue una arquitectura MVC (Modelo–Vista–Controlador), organizada en paquetes para separar responsabilidades y facilitar el mantenimiento.

 app
Contiene las clases principales del modelo de negocio y las entidades del sistema:

Clase	Descripción
Actividades.java	Representa las actividades acuáticas disponibles.
Administrador.java	Hereda de Usuario y gestiona la administración del sistema.
Cliente.java	Hereda de Usuario y representa al cliente que realiza reservas.
Empleados.java	Hereda de Usuario y gestiona las tareas operativas.
MainApp.java	Punto de entrada de la aplicación JavaFX.
Reserva.java	Representa una reserva realizada por un cliente.
Reservable.java	Interfaz que define el comportamiento de los elementos reservables.
Usuario.java	Clase base para todos los tipos de usuario.


 model
Contiene las clases relacionadas con la autenticación y el modelo de datos.

Clase	Descripción
Login.java	Representa las credenciales de acceso y el tipo de usuario.


 mysql
Contiene las clases encargadas de la conexión y comunicación con la base de datos MySQL.

Clase	Descripción
DatabaseConnection.java	Gestiona la conexión con la base de datos.
LoginAccessDB.java	Ejecuta consultas SQL para obtener usuarios y validar credenciales.
TestConexion.java	Clase auxiliar para probar la conexión con MySQL.


 view
Contiene las interfaces gráficas y sus controladores JavaFX.

Archivo / Clase	Descripción
login.fxml	Pantalla de inicio de sesión.

LoginController.java	Controlador que gestiona el proceso de login.

registro.fxml	Pantalla de registro de nuevos usuarios.

RegistroController.java	Controlador que valida y registra usuarios.

reservas.fxml	Pantalla de gestión de reservas.

ReservaController.java	Controlador que maneja la lógica de reservas.

estilos.css	Archivo de estilos visuales.

logo.png	Imagen utilizada en la interfaz.


 util
Contiene utilidades generales del proyecto (por ejemplo, manejo de fechas, validaciones o formatos).

 resources
Directorio reservado para recursos adicionales (imágenes, textos, plantillas, etc.).

4. Diagrama de clases (versión textual)

<img width="1536" height="1024" alt="entidadRelacion" src="https://github.com/user-attachments/assets/be8353bb-fe13-4423-8a80-17b106dfb9c0" />

5. Modelo entidad–relación de la base de datos
   
La base de datos gestor_deportes_acuaticos contiene las siguientes tablas principales:

<img width="570" height="711" alt="image" src="https://github.com/user-attachments/assets/3b357ef7-f2cc-4da8-9c10-fbcbf89646a3" />


7. Manual de usuario
   
 Pantalla de inicio de sesión
 
Permite al usuario acceder introduciendo su nombre y contraseña.

Dependiendo del tipo de usuario (cliente, empleado o administrador), se mostrará una interfaz distinta.

<img width="469" height="625" alt="image" src="https://github.com/user-attachments/assets/b615c8dd-9521-47f8-bc36-21a311dee24d" />

 Pantalla de registro
 
Permite crear nuevos usuarios introduciendo los datos requeridos.

El sistema valida los campos y muestra mensajes de error o confirmación.

<img width="312" height="706" alt="image" src="https://github.com/user-attachments/assets/7eac06bb-8a2e-4e4d-b3b0-aba41882bc6f" />

 Pantalla de reservas
 
Permite visualizar las actividades disponibles y realizar reservas.

Los empleados pueden gestionar las reservas y los administradores supervisarlas.

<img width="348" height="696" alt="image" src="https://github.com/user-attachments/assets/02a1e498-35cc-4dbb-9147-6c8fa412eb82" />

 Pantalla de Administrador
 
 Permite añadir, eliminar o modificar actividades, horarios, monitores y consultar datos.
 
 <img width="615" height="607" alt="image" src="https://github.com/user-attachments/assets/0aa11983-ec80-430e-b7e9-fcb1539a3a56" />


7. Ejecución del proyecto
   
Requisitos

Java 17 instalado

JavaFX configurado

MySQL en ejecución

Archivo launch.json con los argumentos:

--module-path "C:/Users/sergi/Desktop/1DAM/Programación/openjfx-17.0.19_windows-x64_bin-sdk/javafx-sdk-17.0.19/lib" --add-modules javafx.controls,javafx.fxml

Ejecutar la clase:

MainApp.java

9. Autoría

Proyecto desarrollado por Sergio, estudiante del ciclo Desarrollo de Aplicaciones Multiplataforma (DAM), como práctica del módulo de Programación. 
