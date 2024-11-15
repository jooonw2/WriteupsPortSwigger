# File path traversal, validation of file extension with null byte bypass

This lab contains a path traversal vulnerability in the display of product images.

The application validates that the supplied filename ends with the expected file extension.

To solve the lab, retrieve the contents of the `/etc/passwd` file.

Inicializamos la maquina y en una imagen la abrimos en nueva pestaña.

![image.png](image.png)

Ponemos burpsuite a interceptar y recargamos la pagina. Una vez tenemos el paquete lo enviamos al repeater

![image.png](image%201.png)

En este caso no esta validando que termine en jpg.  Ponemos %00. Que lo que hace es ingorarate lo que hay a la derecha pero aun así traga la extensión

![image.png](image%202.png)

![image.png](image%203.png)