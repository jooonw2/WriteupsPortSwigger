# Stored DOM XSS

This lab demonstrates a stored DOM vulnerability in the blog comment 
functionality. To solve this lab, exploit this vulnerability to call the
 `alert()` function.
		
Accedemos a la maquina y entramos a un post. 

![image.png](image.png)

Bajamos hasta el formulario y en el apartado comment ponemos lo siguiente `<><img src=1 onerror=alert(1)>`

![image.png](image%201.png)

Nos sale que se ha guardado el comentario

![image.png](image%202.png)

Volvemos atrás y nos salta la alerta

![image.png](image%203.png)

![image.png](image%204.png)