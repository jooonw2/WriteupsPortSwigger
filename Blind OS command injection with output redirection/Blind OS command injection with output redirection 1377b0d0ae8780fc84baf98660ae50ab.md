# Blind OS command injection with output redirection

Vamos al apartado Submit feedback. Ponemos a interceptar burp y rellenamos el formulario. 

![image.png](image.png)

Ahora tenemos que capturar la salida de whoami y guardarla en la ruta /var/www/images/

||whoami>/var/www/images/output.txt||

Enviamos esto 

![image.png](image%201.png)

Y ahora para verlo vamos a la maquina 

![image.png](image%202.png)

Nos metemos en cualquier articulo, ponemos burp a interceptar y recargamos la pagina. Una vez dentro donde nos sale jpeg lo cambiamos por output.txt

![image.png](image%203.png)

![image.png](image%204.png)