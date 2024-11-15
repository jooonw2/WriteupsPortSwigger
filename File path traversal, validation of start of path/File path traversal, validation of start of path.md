# File path traversal, validation of start of path

This lab contains a path traversal vulnerability in the display of product images.

The application transmits the full file path via a request 
parameter, and validates that the supplied path starts with the expected
 folder.

To solve the lab, retrieve the contents of the `/etc/passwd` file.

Inicializamos la maquina y en una imagen la abrimos en nueva pestaña.

![image.png](image.png)

Ponemos burpsuite a interceptar y recargamos la pagina. Una vez tenemos el paquete lo enviamos al repeater

![image.png](image%201.png)

Deberemos listar el directorio passwd desde la ruta que viene puesta

![image.png](image%202.png)

![image.png](image%203.png)