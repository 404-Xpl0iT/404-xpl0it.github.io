¿Que es un protocolo HTTP?
- HyperText tranducsfer protocol
- Arquitectura cliente - servidor.

¿Que es una URL?
- Partes de las que consta una URL:
	- Protocolo: http (80) o https (443)
	- subdominio y dominio
	- :puerto: podemos elegir el protocolo al que queremos conectarnos, si no lo seleccionamos, se elige por default.
	- Recurso: por ejemplo /index.html, suele encontrarse en la raiz de un servidor web o dentro de un directorio /dir/index.html.

Métodos HTTP
- Método GET: Solicitar datos.
- Método POST: Enviar datos.
- Método PATCH: Modificación parcial de datos.
- Método PUT: Modificación total de datos.
- Método DELETE; Eliminación de recurso.
- Método OPTIONS: Consultar métodos disponibles.
- Método HEAD: Leer cabeceras de respuesta.

Header HTTP
- Host: Nos indica a que host nos vamos a conectar, especificando la ip del servidor o el subdominio o domínio. Tambien podemos definir el puerto.
- User-Agent: Sirve para especificar desde que dispositivo se está conectando el cliente al servidor.
- Accept: Indicamos que tipo de contenido aceptamos en nuestro servidor, por ejemplo: html, txt, xml o si queremos restringir desde el cliente el acceso a algun tipo de recurso.
- Content-Type: A la hora de enviar información al servidor mediante una petición POST, PUT o PATH, le podemos especificar el tipo de datos que estamos enviado con esta cabecera, para que el servidor pueda identificar de manera mas rápida el tipo de información que le estamos enviando.
- Authorization: Cabecera en la que podemos introducir las credenciales encodeadas.
- Cookie: Nos permite especificar nuestra cookie de sesión o cualquier otro tipo de cookie en la que podemos tener información como nuestro id de usuario.

Body-Request HTTP
- El body es la información que enviamos a la web para añadir un nuevo recurso o modificar uno existente.
- username, password, etc...

Códigos de Estado HTTP (Respuestas HTTP)
- 1xx: informativos.
- 2xx: Success
- 3xx: Redirect
- 4xx: Client error
- 5xx: Server error

Headers de respuesta
- Server: Te muestra el servicio que corre por detras de la web.
- X-Powered-By: Informa que version de PHP está funcionando.
- Location: Te indica a donde te redirecciona el redirect al ser un codigo 302.
- Content-Type: Indica que tipo de contenido está dando en el body la web.

Body de Respuesta
- Aparece el contenido de la web.

Cookies HTTP
- Son pequeños fragmentos de datos que nos envia el servidor web a nuestro navegador para que almacenemos información temporalmente o para siempre.
- Diferentes usos de cookies:
	- Cookies de Autenticación: Encargadas de gestionar las sesiones del usuario. Tu al loguearte en una web, el servidor te da una cookie y de esa forma no hay que estar constantemente iniciando sesión en la web para hacer cualquier tipo de gestión.
	- Cookies de seguimiento/personalización: Sirven para rastrear el comportamiento del usuario y personalizar la experiencia. Podemos decirle a una web en la que no hemos iniciado sesión que queremos cambiar el color para tener esa personalización por ejemplo y se guardarían en el navegador, asi que cada vez que entremos en esa web, se cargarían estas preferencias.
	- Cookies de carritos de compra: Los artículos que añadimos al carrito quedan almacenados en tus cookies para no tener que volver a meterlos en el carrito si abandonas la web.
- Diferentes tipos de cookies:
	- Cookies de sesión: Se almacenan en el navegador pero si lo cierras, el navegador las elimina.
	- Cookies persistentes: Permanecen en el dispositivo hasta que tu las eliminas o expiran. Sirven para mantenerte autenticado durante un largo periodo de tiempo.
	- Cookies de terceros: Cuando haces unas búsquedas de algo, te sale publicidad de esos productos que has buscado.
