<p align="center"><a href="https://laravel.com" target="_blank"><img src="https://raw.githubusercontent.com/laravel/art/master/logo-lockup/5%20SVG/2%20CMYK/1%20Full%20Color/laravel-logolockup-cmyk-red.svg" width="400" alt="Laravel Logo"></a></p>

Este laboratorio se desarrolló utilizando el framework Laravel, basado en la arquitectura MVC, la cual permite separar la lógica de la aplicación en tres componentes principales:

Modelos (app/Models): Gestionan la lógica de datos y la interacción con la base de datos.
Vistas (resources/views): Se encargan de la interfaz gráfica que ve el usuario.
Controladores (app/Http/Controllers): Procesan las solicitudes y conectan modelos con vistas.
Rutas (routes/web.php): Definen las URLs y su comportamiento.

EL obejtivo de este laboratorio es aplicar la arquitectura MVC mediante Laravel, implementando autenticación, manejo de base de datos y configuración del entorno de desarrollo.

 Prerrequisitos: (ecosistema de desarrollo del lab)
▪ PHP versión 8.0 o superior.
▪ Composer última versión estable.
▪ Laravel Installer o crear proyecto con laravel new /
composer create-project.
▪ Paquete de servidor web local. (Entorno de Desarrollo)(ej.
XAMPP, WampServer o Laragon).
▪ Servidor web: Apache o Nginx
▪ Base de datos MySQL/MariaDB funcionando.
▪ Editor de código (Visual Studio Code recomendado).
▪ NPN: si fue necesario. Dejarlo en blanco de lo Contrario.
▪ Sistema Operativo:
▪ Incluir iconos por Tecnología
▪ Instalación de dependencias con composer install y configuración del
archivo .env. Secuencia de Comandos utilizados. 

Laravel/ui
Coposer require laravel/ui
Php artisan ui Bootstrap –auth
Npm install && npm run dev

Ejecucion:
<img width="1891" height="914" alt="image" src="https://github.com/user-attachments/assets/39198b7d-ef50-4a54-a36c-a0fab796f033" />
<img width="1889" height="911" alt="image" src="https://github.com/user-attachments/assets/cc5cc57c-4e38-43e3-b04a-803b6091e1f0" />

Base de datos

Se configuró en el archivo .env con MySQL.
Las tablas fueron generadas mediante migraciones de Laravel.

Ejemplo:
DB_DATABASE=labloginlaravel
DB_USERNAME=root
DB_PASSWORD=

Dificultades y soluciones

Error: tabla sessions no existe
Problema: Laravel intentaba usar sesiones en base de datos sin tener la tabla creada.
Solución:
aplique el comando php artisan migrate: refresh
esto actualizaba la base de datos lo cual en mi caso quito el problema.

Este laboratorio ha sido desarrollado por el estudiante de la Universidad
Tecnológica de Panamá:
Nombre: Abraham Alcedo
Correo: abraham.alcedo@utp.ac.pa
Curso: IGS131
Instructor del Laboratorio: Irina Fong.
con fecha 15/4/2026
