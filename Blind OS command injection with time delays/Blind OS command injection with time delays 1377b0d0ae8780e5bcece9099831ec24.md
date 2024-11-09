# Blind OS command injection with time delays

Vamos al apartado submit feedback

![image.png](image.png)

Ponemos burp a escuchar y rellenamos el formulario

![image.png](image%201.png)

Ahora vamos a mandar el comando que nos ha mandado, un ping con un delay de  10 segundos. Ponemos lo siguiente y le damos a Forward

`||ping+-c+10+127.0.0.1||`

También podemos hacerlo con:

`||sleep+10||`

![image.png](image%202.png)

Ya estaria

![image.png](image%203.png)