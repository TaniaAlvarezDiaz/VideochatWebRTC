# VideochatWebRTC
Aplicación de videochat utilizando [WebRTC](https://webrtc.org/). Esta aplicación tiene:
 - [Servidor](https://github.com/TaniaAlvarezDiaz/VideochatWebRTCServidor): se encarga de gestionar las conexiones de los usuarios.
 - [Cliente](https://github.com/TaniaAlvarezDiaz/VideochatWebRTCCliente): permite a los usuarios conectarse al servidor y realizar el intercambio de video y mensajes de chat con el resto de usuarios conectados al servidor (usando el nombre de dicho usuario).
 
Adicionalmente, en este repositorio se hace referencia a la documentación de la aplicación.

# Ejecución

Para ejecutar el proyecto seguir los siguientes pasos:
1. Descargar [Node.js](https://nodejs.org/es/)

2. Descargar el proyecto:
   * git clone https://github.com/TaniaAlvarezDiaz/VideochatWebRTC.git
   * Acceder a la carpeta y ejecutar:
      * git submodule update --init

3. Ejecutar la consola de Node.js.
   * Ir a la ruta donde se encuentra el servidor (**VideochatWebRTCServidor**).
   * Ejecutar "node server.js".
   
4. Ir a la ruta donde se encuentra el cliente (**VideochatWebRTCCliente**). Hay dos posibilidades de ejecución:
   * Abrir el fichero "index.html" en el navegador Chrome.
      * Arrancar Chrome con la directiva **allow file access from files**.
      * Abrir tantas pestañas como clientes se deseen.
   * Desplegar el cliente desde un servidor. Si no se posee de uno, se aconseja utilizar [XAMPP](https://www.apachefriends.org/es/index.html) (continuar viendo paso 5).
   
5. Si se utiliza XAMPP para desplegar el cliente, tras instalarlo se debe:
   * Introducir el cliente (carpeta **VideochatWebRTCCliente**) en la carpeta "htdocs".
      * Se suele encontrar en la ruta "C:\xampp\htdocs". 
   * Desde el panel de XAMPP, iniciar el servicio de Apache pulsando "Run".
      * Habitualmente este servicio se inicia en el puerto 80.
   * Abrir el navegador Chrome y ejecutar **localhost/VideochatWebRTCCliente**.
      * Si el puerto no es el 80, se ejecutaría **localhost:PUERTO/VideochatWebRTCCliente**, donde PUERTO es el número del puerto.
 
