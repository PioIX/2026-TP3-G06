##2026-TP3-G06

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

**Ejemplo de comunicación**
Cuando un usuario inicia sesión, el navegador envía los datos al servidor. El servidor verifica la información y devuelve una respuesta indicando si el inicio de sesión fue correcto o no.
