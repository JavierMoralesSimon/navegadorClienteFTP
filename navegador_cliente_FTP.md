# Uso del navegador como cliente FTP

## Acceso al servidor FTP desde un navegador
Debido a que varios navegadores modernos han eliminado el soporte nativo para el protocolo FTP por motivos de seguridad, si tratamos de acceder al servidor desde aquí habiendo previamente puesto a correr el servidor en FileZilla Server Administration, y luego poniendo en la url "ftp://" más la ip (en mi caso uso el usuario anonymouse por lo que no debo de especificar usuario y contraseña) no nos dejará y se nos indicará que usemos un complemento para poder realizar la tarea, dejando al navegador actuando simplemente como un "puente".
![Acceso al servidor FTP desde un navegador](https://github.com/JavierMoralesSimon/navegadorClienteFTP/blob/main/Capturas/1.png)

## Limitaciones frente a un cliente dedicado
Generamos la misma conexión que antes pero a través de FileZilla Client, dando éxito.
![Limitaciones frente a un cliente dedicado](https://github.com/JavierMoralesSimon/navegadorClienteFTP/blob/main/Capturas/2.png)

Las limitaciones serían:
* Subida de archivos: En el navegador web es generalmente imposible (solo lectura), mientras que el cliente dedicado se ofrece soporte total mediante "Drag & Drop".
* Gestión de carpetas: El navegador web no permite crear ni borrar carpetas, a diferencia del cliente dedicado, que permite un control total del sistema de archivos.
* Seguridad (FTPS/SFTP): En el navegador web es muy limitada o inexistente; por el contrario, el cliente dedicado soporta cifrado avanzado y gestión de certificados.
* Transferencia masiva: El navegador web solo permite descargar archivos uno a uno, mientras que el cliente dedicado permite gestionar colas de miles de archivos simultáneamente.
* Reanudación: Si la descarga se corta en el navegador web, suele fallar y debe reiniciarse, pero el cliente dedicado permite reanudar transferencias interrumpidas desde donde se quedaron.
* Interfaz: El navegador web muestra una interfaz rudimentaria (simple lista de enlaces), mientras que el cliente dedicado utiliza una interfaz de doble panel para gestionar el sitio local vs el remoto.

## Ventajas y desventajas del navegador como cliente FTP
* Ventajas:
  * Ubicuidad y conveniencia: No requiere instalar software adicional; casi cualquier dispositivo tiene un navegador.
  * Curva de aprendizaje cero: Cualquier usuario sabe hacer clic en un enlace de una lista para descargar un archivo.
  * Rapidez para descargas puntuales: Es ideal para descargar un único manual o driver sin configurar perfiles de conexión complejos.
  * Previsualización básica: Algunos navegadores permiten abrir archivos de texto o imágenes directamente en la pestaña antes de guardarlos.

* Desventajas
  * Protocolo "zombie": La mayoría de navegadores modernos han desactivado el soporte nativo, obligando a usar extensiones o aplicaciones externas.
  * Inseguridad: Rara vez soportan FTPS, lo que significa que tus credenciales y datos viajan por la red de forma legible para atacantes.
  * Unidireccionalidad: Está diseñado casi exclusivamente para la descarga. La subida de archivos es complicada o imposible.
  * Inestabilidad en archivos grandes: Carece de algoritmos de verificación de integridad y de reanudación automática si la conexión oscila.
  * Gestión inexistente: No permite cambiar permisos, renombrar archivos en el servidor o editar código en tiempo real.
