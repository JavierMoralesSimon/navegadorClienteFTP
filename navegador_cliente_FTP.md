# Uso del navegador como cliente FTP

## Acceso al servidor FTP desde un navegador
Debido a que varios navegadores modernos han eliminado el soporte nativo para el protocolo FTP por motivos de seguridad, si tratamos de acceder al servidor desde aquí habiendo previamente puesto a correr el servidor en FileZilla Server Administration, y luego poniendo en la url "ftp://" más la ip (en mi caso uso el usuario anonymouse por lo que no debo de especificar usuario y contraseña) no nos dejará y se nos indicará que usemos un complemento para poder realizar la tarea.
![Acceso al servidor FTP desde un navegador](https://github.com/JavierMoralesSimon/navegadorClienteFTP/blob/main/Capturas/1.png)

## Limitaciones frente a un cliente dedicado
![Limitaciones frente a un cliente dedicado](https://github.com/JavierMoralesSimon/navegadorClienteFTP/blob/main/Capturas/2.png)

## Ventajas y desventajas del navegador como cliente FTP
* Subida de archivos: En el navegador web es generalmente imposible (solo lectura), mientras que el cliente dedicado se ofrece soporte total mediante "Drag & Drop".
* Gestión de carpetas: El navegador web no permite crear ni borrar carpetas, a diferencia del cliente dedicado, que permite un control total del sistema de archivos.
* Seguridad (FTPS/SFTP): En el navegador web es muy limitada o inexistente; por el contrario, el cliente dedicado soporta cifrado avanzado y gestión de certificados.
* Transferencia masiva: El navegador web solo permite descargar archivos uno a uno, mientras que el cliente dedicado permite gestionar colas de miles de archivos simultáneamente.
* Reanudación: Si la descarga se corta en el navegador web, suele fallar y debe reiniciarse, pero el cliente dedicado permite reanudar transferencias interrumpidas desde donde se quedaron.
* Interfaz: El navegador web muestra una interfaz rudimentaria (simple lista de enlaces), mientras que el cliente dedicado utiliza una interfaz de doble panel para gestionar el sitio local vs el remoto.
