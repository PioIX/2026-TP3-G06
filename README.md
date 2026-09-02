##2026-TP3-G06
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

**Ejemplo de comunicación**
Cuando un usuario inicia sesión, el navegador envía los datos al servidor. El servidor verifica la información y devuelve una respuesta indicando si el inicio de sesión fue correcto o no.

#PARTE 3
# El Back-End (Servidor) y Base de Datos

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
