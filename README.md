
# PARTE 1
# **Introducción a las Aplicaciones Web y Arquitectura Cliente-Servidor**

## **¿Qué es una aplicación web?**
Una aplicación web es un software al que se accede mediante un navegador web y que permite al usuario realizar diferentes acciones, como iniciar sesión, completar formularios, realizar compras o gestionar información.

## **Diferencia entre una aplicación web y un sitio web estático**
Un sitio web estático muestra información que generalmente es igual para todos los usuarios y cuyo contenido cambia poco. Por ejemplo, una página informativa de una empresa.

En cambio, una aplicación web permite una mayor interacción con el usuario y puede procesar y almacenar información. Por ejemplo, una tienda online, un sistema de gestión o un correo electrónico.

## **Modelo Cliente-Servidor**
El modelo Cliente-Servidor es una arquitectura en la que un cliente realiza solicitudes y un servidor las recibe, procesa y devuelve una respuesta.

## **Cliente (Navegador)**
El cliente es el navegador web que utiliza el usuario, como Google Chrome, Mozilla Firefox o Microsoft Edge. Su función es enviar solicitudes al servidor y mostrar la información que recibe.

## **Servidor**
El servidor recibe las solicitudes del cliente, procesa la información y devuelve una respuesta. También puede encargarse de acceder a bases de datos y realizar diferentes operaciones.

## **Ejemplo de comunicación**
Cuando un usuario inicia sesión, el navegador envía los datos al servidor. El servidor verifica la información y devuelve una respuesta indicando si el inicio de sesión fue correcto o no.


# PARTE 2
# FRONT-END (CLIENTE)
Es la parte de una aplicación web con la que el usuario interactúa directamente visual y funcionalmente en su navegador (como Chrome, Firefox o Edge).

### Tecnologías Fundamentales
La interfaz web se construye combinando tres tecnologías principales:

- **HTML (HyperText Markup Language):** Define la estructura y el contenido de la página (títulos, párrafos, imágenes, formularios, botones).

- **CSS (Cascading Style Sheets):** Define la presentación visual, el diseño, los colores, la tipografía y el comportamiento adaptativo (Responsive Design) para distintas pantallas.

- **JavaScript:** Agrega interactividad dinámica a la aplicación, permitiendo responder a eventos del usuario (clics, desplazamientos), validar formularios en tiempo real y actualizar contenido sin recargar la página.

### El Navegador Web y el Motor de Renderizado

El navegador actúa como el entorno de ejecución del cliente. Su trabajo principal es transformar el código recibido desde el servidor en una interfaz visual ejecutable:

- **Recepción del código:** El navegador realiza una petición al servidor y recibe los archivos .html, .css y .js.

- **Construcción del DOM (Document Object Model):** El navegador lee el HTML y genera una estructura de árbol en memoria que representa los elementos de la página.

- **Construcción del CSSOM (CSS Object Model):** Interpreta los estilos CSS y determina cómo debe verse cada elemento del DOM.

- **Árbol de Renderizado (Render Tree):** Combina el DOM y el CSSOM para calcular qué elementos son visibles y cómo se ubican en la pantalla (Layout).

- **Ejecución de JavaScript:** El motor del navegador (como V8 en Chrome) ejecuta el código JS, lo que puede modificar el DOM o el CSSOM en tiempo real y desencadenar un nuevo renderizado.

### Renderizado en el Cliente (Client-Side Rendering vs. Server-Side Rendering)
Existen dos enfoques principales sobre cómo se genera la interfaz:

- **Server-Side Rendering (SSR):** El servidor genera el HTML completo y se lo envía listo al navegador. Cada cambio de página suele requerir una nueva descarga completa.

- **Client-Side Rendering (CSR):** El servidor envía un HTML casi vacío junto con archivos de JavaScript. El navegador descarga el JavaScript y este se encarga de construir la interfaz y solicitar solo los datos necesarios (por ejemplo, mediante llamadas a APIs en formato JSON). Este enfoque es la base de las aplicaciones de una sola página (Single Page Applications o SPAs) construidas con frameworks como React, Angular o Vue.

# PARTE 3
## El Back-End (Servidor) y Base de Datos

## ** ¿Qué es el Back-End?**
El Back-End es la parte de una aplicación web que funciona en el servidor y se encarga de procesar las solicitudes del usuario. También contiene la lógica necesaria para realizar operaciones, gestionar información y comunicarse con la base de datos.

## **Función del servidor web y de aplicaciones**
El servidor web recibe las solicitudes que realiza el navegador y devuelve los recursos correspondientes, como páginas, archivos o respuestas.

El servidor de aplicaciones se encarga de ejecutar la lógica de la aplicación. Procesa las solicitudes, realiza operaciones y genera las respuestas que serán enviadas al cliente.

## **Lógica de negocio**
La lógica de negocio contiene las reglas y procesos que determinan cómo debe funcionar la aplicación.

Por ejemplo, en una tienda online, la lógica de negocio puede comprobar si un producto tiene stock antes de permitir que el usuario realice una compra.

## **Interacción con la base de datos**
El Back-End se comunica con la base de datos para consultar, guardar, modificar o eliminar información.

**Ejemplo,** cuando un usuario inicia sesión, el servidor puede consultar la base de datos para comprobar si el correo y la contraseña corresponden a un usuario registrado.

También puede guardar información nueva. Por ejemplo, cuando un usuario crea una cuenta, el servidor recibe sus datos y los almacena en la base de datos.

## **Flujo de información**
Cuando un usuario realiza una acción desde el navegador, este envía una solicitud al servidor o Back-End. El servidor recibe la solicitud y procesa la información utilizando la lógica de negocio de la aplicación. Si es necesario, el Back-End se comunica con la base de datos para consultar, guardar, modificar o eliminar información.

Una vez realizado el proceso, la base de datos devuelve la información al Back-End. El servidor procesa los datos y envía una respuesta al navegador, donde finalmente se muestra el resultado al usuario.

De esta manera, el Back-End funciona como intermediario entre el usuario y la base de datos, procesando las solicitudes y aplicando las reglas necesarias antes de devolver una respuesta.

# PARTE 4
## Protocolo HTTP/HTTPS y el Ciclo Request-Response

El **Protocolo HTTP/HTTPS** es el conjunto de reglas que permite la comunicación y el intercambio de datos entre el navegador (cliente) y el servidor web.

### Ciclo Request-Response (Petición - Respuesta)
1. **Petición (Request):** El navegador envía una solicitud al servidor pidiendo un recurso (una página, una imagen o datos).
2. **Procesamiento:** El servidor recibe la petición, busca la información o ejecuta la lógica necesaria.
3. **Respuesta (Response):** El servidor responde al navegador enviando el código correspondiente (HTML, JSON) junto con un código de estado.

### Métodos HTTP principales
* **GET:** Solicita información al servidor sin modificarla.
* **POST:** Envía datos al servidor para crear un nuevo recurso (ej. enviar un formulario).
* **PUT / PATCH:** Actualiza información existente en el servidor.
* **DELETE:** Elimina un recurso en el servidor.

### Códigos de estado más comunes
* **200 OK:** La solicitud fue exitosa.
* **301 / 302:** Redirección a otra dirección.
* **404 Not Found:** El recurso solicitado no existe.
* **500 Internal Server Error:** Ocurrió un error dentro del servidor.

### Seguridad: HTTP vs. HTTPS
* **HTTP:** Transmite la información en texto plano, lo que la hace vulnerable a interceptaciones.
* **HTTPS:** Utiliza cifrado (mediante certificados SSL/TLS) para proteger los datos durante el trayecto, garantizando privacidad y autenticidad.
