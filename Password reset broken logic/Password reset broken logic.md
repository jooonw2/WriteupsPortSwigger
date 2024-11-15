# Password reset broken logic

This lab's password reset functionality is vulnerable. To solve the lab, reset Carlos's password then log in and access his "My account" page.

- Your credentials: `wiener:peter`
- Victim's username: `carlos`

Accedemos a la maquina, vamos al apartado de My account.

![image.png](image.png)

Y le damos a que hemos olvidado la contraseña.

![image.png](image%201.png)

Ponemos el usuario wiener

![image.png](image%202.png)

Vamos al apartado Email client

![image.png](image%203.png)

Vemos que nos ha llegado esto

![image.png](image%204.png)

Vamos al link y metemos la nueva contraseña. Antes ponemos burpsuite a escuchar

![image.png](image%205.png)

Localizamos este paquete y lo enviamos al repeater

![image.png](image%206.png)

Borramos la nueva contraseña

![image.png](image%207.png)

Y ahora cambiamos el usuario

![image.png](image%208.png)

Y se nos cambia la contraseña y vemos que podemos acceder.

![image.png](image%209.png)