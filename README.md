Pasos para hacer las pruebas:

1-	Haz click al botón de <> Codey selecciona abrir con Visual Studio o también puede descargarlo, descomprimir y luego abrirlo en Visual Studio.
2-	Correr el script de creación BD en Sql Server Manament Studio
3-	Cambiar el valor del parámetro Data Source en la cadena de conexión, que se encuentra en el controlador CreacionUsuarioController.cs, por el server name del Sql Server Manament Studio instalado en la maquina donde se probara el proyecto.
4-	Ejecuta el proyecto en Visual Studio, como se implemento Swagger el mismo se ejecutará desde ahí, donde se podrá hacer las pruebas de la API.
5-	Ejecutar el método de login, el mismo cuenta con los datos de login de un usuario defecto, ya creado en la BD en el paso 2. Este devolverá un Jwt Token.
6-	Ingresa al método de Creación, que pedirá el token generado en el paso anterior y el correo que se usó en el login. Luego de esto podrá crear el usuario en la BD usando el Json que se encuentra en el Request body (puede modificarlos por los valores deseados). Luego de esto se mostrarán los datos del usuario registrado, incluyendo un token que luego puede usar ese correo para crear para otro usuario o bien hacer el login y obtener un nuevo token.
 
