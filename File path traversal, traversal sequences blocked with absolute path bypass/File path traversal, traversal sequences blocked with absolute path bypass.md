# File path traversal, traversal sequences blocked with absolute path bypass

This lab contains a path traversal vulnerability in the display of product images.

The application blocks traversal sequences but treats the 
supplied filename as being relative to a default working directory.

To solve the lab, retrieve the contents of the `/etc/passwd` file.

Inicializamos la maquina y en una imagen la abrimos en nueva pestaña.

![image.png](image.png)

Ponemos burpsuite a interceptar y recargamos la pagina. Una vez tenemos el paquete lo enviamos al repeater

![image.png](image%201.png)

En filename ponemos directamente /etc/passwd Ya que esta cargando los directorios desde la raiz

![image.png](image%202.png)

![image.png](image%203.png)