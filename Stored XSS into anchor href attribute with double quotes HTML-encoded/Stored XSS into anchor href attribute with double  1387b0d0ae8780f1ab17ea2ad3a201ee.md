# Stored XSS into anchor href attribute with double quotes HTML-encoded

This lab contains a stored cross-site scripting vulnerability in the 
comment functionality. To solve this lab, submit a comment that calls 
the `alert` function when the comment author name is clicked.
        
Accedemos al laboratorio y accedemos a un post. Ponemos burpsuite a escuchar. Y rellenamos el formulario

![image.png](image.png)

Interceptamos el paquete y lo mandamos al repeater, ya que lo usaremos luego 

![image.png](image%201.png)

Como vemos en la maquina se nos ha añadido

![image.png](image%202.png)

Ponemos burpsuite a escuchar y hacemos clic sobre el nombre de usuario del comentario que hemos añadido

![image.png](image%203.png)

El paquete que hemos interceptado lo mandamos al repeater. Tenemos los dos paquetes

![image.png](image%204.png)

Añadimos lo siguiente `javascript:alert(1)` y lo enviamos

![image.png](image%205.png)

![image.png](image%206.png)

Podemos ver que se nos ha añadido un ultimo comentario que si hacemos clic sobre el nos salta la alerta

![image.png](image%207.png)