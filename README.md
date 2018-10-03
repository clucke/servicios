# servicios
Para instalar servicios solo hay que copiar la carpeta a htdocs en caso de xampp y html de apache2, dentro de la carpeta servicios contiene una carpeta config y dentro un archivo config.php, modificar el archivo con los datos a la conexion que va a utilizar, para probar el funcionamiento ejecute http://localhost/servicios/public/
o http://[ip]/servicios/public/ debe de aparecer en el navegador Method not allowed.
Para ejecutar pruebas unitarias es necesario abrir la terminal, ubicarse en la raiz de la carpeta servicios y ejecutar ./vendor/bin/phpunit ./test/test.php 
Probar con postman, enviar un json 
{
	"servicio":"usuarios",
	"opcion":4
} 
por post en la ruta de servicios + /public, es decir, si servicios se encuentra en http://localhost/servicios colocar /public, quedaria http://localhost/servicios/public

Nota: es necesario tener descomentado extension=php_pdo_mysql.dll en el archivo php.ini.