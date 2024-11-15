# File path traversal, traversal sequences stripped non-recursively

Iniciamos la maquina, ponemos burp a interceptar y entramos en un post.

![image.png](image.png)

Ahora le damos a Forward hasta poder atrapar este paquete. Y lo mandamos al repeater

![image.png](image%201.png)

Ponemos lo siguiente ….//….//….//etc/passwd. Ponemos 4 puntos ya que nos borra 2

![image.png](image%202.png)

Y recargamos la pagina

![image.png](image%203.png)