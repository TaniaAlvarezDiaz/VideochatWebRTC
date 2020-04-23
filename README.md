# VideochatWebRTC
Aplicación de videochat que permite a los usuarios comunicarse entre sí mediante el intercambio de vídeo y mensajes de chat.. Esta aplicación tiene:
 - [Servidor](https://github.com/TaniaAlvarezDiaz/VideochatWebRTCServidor): se encarga de gestionar las conexiones de los usuarios.
 - [Cliente](https://github.com/TaniaAlvarezDiaz/VideochatWebRTCCliente): permite a los usuarios conectarse al servidor y realizar el intercambio de video y mensajes de chat con el resto de usuarios conectados al servidor (usando el nombre de dicho usuario).
 
Adicionalmente, en este repositorio se hace referencia a la documentación de la aplicación.

# Ejecución

Para ejecutar el proyecto seguir los siguientes pasos:
1. Descargar [Node.js](https://nodejs.org/es/)

2. Descargar el proyecto:
   * git clone --recurse-submodules https://github.com/TaniaAlvarezDiaz/VideochatWebRTC.git

3. Ejecutar la consola de Node.js.
   * Ir a la ruta donde se encuentra el servidor (**VideochatWebRTCServidor**).
   * Ejecutar "node server.js".
   
4. Ir a la ruta donde se encuentra el cliente (**VideochatWebRTCCliente**).
   * Abrir el fichero "index.html" en el navegador Chrome.
      * Abrir tantas pestañas como clientes se deseen.
   * **Nota**: puede ser que el navegador Chrome bloquee alguna característica de Javascript que sea necesaria para la correcta ejecución si se abre el archivo "index.html" desde una ruta local, por tanto, es recomendable desplegar el cliente desde un servidor.
   Si no se posee de uno, se aconseja utilizar [Xampp](https://www.apachefriends.org/es/index.html) (continuar viendo paso 5).
   
5. Si se utiliza Xampp para desplegar el cliente, tras instalarlo se debe:
   * Introducir el cliente (carpeta **VideochatWebRTCCliente**) en la carpeta "htdocs".
      * Se suele encontrar en la ruta "C:\xampp\htdocs". 
   * Desde el panel de Xampp, iniciar el servicio de Apache pulsando "Run".
      * Habitualmente este servicio se inicia en el puerto 80.
   * Abrir el navegador Chrome y ejecutar **localhost/VideochatWebRTCCliente**.
      * Si el puerto no es el 80, se ejecutaría **localhost:PUERTO/VideochatWebRTCCliente**, donde PUERTO es el número del puerto.
   

